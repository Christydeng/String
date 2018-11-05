# String
字符串的使用


1. 长度超出改用'...'显示(tips: 可以利用字符串的长度属性 length 以及使用三目运算符)

    function soution(string, limit){
        return string.length>limit?string.substr(0, limit)+'...' : string
    }
    
 2. 超长数字用逗号分隔 例： 1234567 =>  1，234，567
    
    let str = '1234567';
    //  因为数组才有reverse方法，所以在反转之间要先把字符串分割（split）成数组，反转之后再拼接（join）变成字符串。
    let newStr = str.split('').reverse.join();
    let temp = '';
    for (let i = 0; i < newStr.length; i++) {
        if (i % 3 === 0 && i !==0) {
            temp += ',';
        }
        temp += newStr.chatAt(i);
    }
    let result = temp.split('').reverse().join();
    
 
    
    
