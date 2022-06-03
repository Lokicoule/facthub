# UC_SETTING_GENERATE_CODE

A. Actors

- User

B. Used by

- Customer
- Product
- Order
- Transporter
- Warehouse

C. Description

Business code has to be generated if is empty.

- Use case value is `CODE_GENERATOR`
- There are 3 types of parameters
  - `PREFIX` [BR_SETTING_PREFIX_PARAM](#brsettingprefixparam)
  - `COUNTER` [BR_SETTING_COUNTER_PARAM](#brsettingcounterparam)
  - `SUFFIX` [BR_SETTING_SUFFIX_PARAM](#brsettingsuffixparam)

C. Basic Flow

1. Use case begins when Actors start create action with empty code.
2. [BR_SETTING_GENERATE_CODE_FROM_PARAMS](#brsettinggeneratecodefromparams)
3. Use case ends when generated code is return.

---

# Business Rules

### BR_SETTING_PREFIX_PARAM

- Prefix parameter key can be null or empty

### BR_SETTING_COUNTER_PARAM

- Counter parameter key must exists
- Counter parameter value accepts only digit character

### BR_SETTING_SUFFIX_PARAM

- Suffix parameter must exists

### BR_SETTING_GENERATE_CODE_FROM_PARAMS

- concatenation order
  1. PREFIX
  2. COUNTER
  3. SUFFIX
- examples

  ```
  Input 1
    prefix = "2022#"
    counter = "00001"

  Output 1
    2022#00001

  Input 2
    prefix = "2022"
    counter = "00001"
    suffix = "#"

  Output 2
    202200001#

  Input 3
    counter = "00001"
    suffix = "#F"

  Output 3
    00001#F
  ```
