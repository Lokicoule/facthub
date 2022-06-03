# Counter business rules

## BR_SETTING_COUNTER_PARAM_INCREMENT_BY_ONE

Counter should be incremented by one.

```
Input
00001
Output
00002
```

## BR_SETTING_COUNTER_PARAM_INCREMENT_WITH_LEADING_ZERO

counter should respect leading zero

Examples :

```
Input 1
00009
Output 1
00010

Input 2
00099
Output 2
00100
```
