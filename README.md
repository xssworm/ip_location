ip_location
===========

It's a hhvm extension that you give an ip which will return an array of address.

compile:
```
hphpize
cmake . && make
```

test:
```
hhvm -vDynamicExtensions.0=ip_location.so test.php
```

output:
```
0.000076
array(5) {
  ["country"]=>
  string(2) "CN"
  ["province"]=>
  string(6) "北京"
  ["area"]=>
  string(6) "北京"
  ["city"]=>
  string(6) "海淀"
  ["isp"]=>
  string(6) "UNICOM"
}
```
