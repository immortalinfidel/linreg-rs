# Linear Regression (linreg)
```
use linreg_rs::LinReg;
use ta_common::traits::Indicator;

let mut linreg = LinReg::new(5);
assert_eq!(linreg.next(81.59), None);
assert_eq!(linreg.next(81.06), None);
assert_eq!(linreg.next(82.87), None);
assert_eq!(linreg.next(83.00), None);
assert_eq!(linreg.next(83.61), Some(83.622));
assert_eq!(linreg.next(83.15), Some(83.72199999999998));
assert_eq!(linreg.next(82.84), Some(83.11199999999998));
assert_eq!(linreg.next(83.99), Some(83.55999999999997));
assert_eq!(linreg.next(84.55), Some(84.17199999999997));
assert_eq!(linreg.next(84.36), Some(84.60399999999998));
assert_eq!(linreg.next(85.53), Some(85.40399999999998));
assert_eq!(linreg.next(86.54), Some(86.20999999999998));
assert_eq!(linreg.next(86.89), Some(86.94599999999997));
assert_eq!(linreg.next(87.77), Some(87.85399999999996));
assert_eq!(linreg.next(87.29), Some(87.75399999999996));


```