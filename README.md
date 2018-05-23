# Q.OneNumberInputAndOutputTheSumOfEachDigit


## *정수 하나를 입력받아 각 자리수 숫자들의 합을 반환해주는 함수*

````
func sdaf(n:Int){
    var total = 0
    var c = n % 10
    var b = (n/10) % 10
    var a = (n/10)/10
    total = a + b + c
    
print(a, b, c)
print(total)
}
sdaf(n: 123)
sdaf(n: 45)
````

````
func addNum(_ num : Int)-> Int{
    var count = 1
    var sum = 0
    var newNum = 0
    var firstNum:Int
    firstNum=num

    while num > count{
        count *= 10
    }

    while count >= 1{
        newNum = firstNum/count
        sum += newNum
        firstNum = firstNum - (newNum * count)
        count /= 10
    }

    return sum
}

addNum(123)
addNum(1)
addNum(6463)
````

````
func addFn(_ num: Int) -> Int{
    var addTemp: Int = num
    var result: Int = 0

    while addTemp > 0 {
        result += addTemp % 10
        addTemp = addTemp / 10
    }
    return result

}

print(addFn(123))
````
