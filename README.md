# KDB/Q

## Download && Install
   * Unzip the package and check directory structure and files.
```
$ ls -R q
q:
README.txt  q.k  q.q  s.k  sp.q  trade.q  w32

q/w32:
q.exe

```
   * Set up env var _QHOME_ and _PATH_

## Start up
```
$ q
...
q)til 3
0 1 2
q)"c"$0x57656c6c20646f6e6521
"Well done!"
```
## Variables
```
q)a:42
q)a
42
q)show a
42
q)show a:42
42
```
## Order of Evaluation
q)show b:1+a:42
43
q)a
42
q)b
43
```
' / ' to comment 
```
q)show b:1+a:42 / nothing here counts c:6*7
43
q)c
'c
  [0]  c
       ^
q)
```
