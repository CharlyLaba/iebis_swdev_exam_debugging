# Bug Report and Correction

## Bug 1

``` 
switch (random.nextInt(2)) {
```
It should be replaced by 3 since there are 3 cases, not 2.

> Correction
```
switch (random.nextInt(3)) {
```

## Bug 2

```
                   case 0:
                word = new StringBuffer('Y');
                   case 1:
                word = new StringBuffer('F');
                   case 2:
                word = new StringBuffer('T');
``` 
                
The letters should be in double quotation since they are literal Strings s and not literal Char s 

```
                   case 0:
                word = new StringBuffer("Y");
                   case 1:
                word = new StringBuffer("F");
                   case 2:
                word = new StringBuffer("T");
 ``` 
  ## Bug 3
  We must introduce the breaks after each option so it can complete the entire code without skipping the first two and just outputting the last one. 
  
 ``` 
           switch (random.nextInt(3)) {
                    case 0:
                word = new StringBuffer("Y");
            break; case 1:
                word = new StringBuffer("F");
            break; case 2:
                word = new StringBuffer("T");
                break;
        }
                
 ``` 
                
       
