# How to set default arguments value to function

    function volume(a, b = 3, c = 4) {
        return a * b * c;
    }

## Example of funtion calling with different arguments

### 1 : Function with 3 argument value
    let vol = volume(2,4,5);
    console.log(vol)
    Output : 40

### 2 : Function with 2 argument value
    let vol = volume(2,4);
    console.log(vol)
    Output : 32

### 3 : Function with 1 argument value
    let vol = volume(2);
    console.log(vol)
    Output : 24

## **Note**
 If no arguments pass then function will return NAN \
 Number multiplied by undefined will return NAN \
    <b>Reason : </b> vol() \
    a = undefined , b = 3 , c = 4 \
    undefined * 3 * 4  = **NAN**
