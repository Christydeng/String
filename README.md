# String
字符串的使用


1. 长度超出改用'...'显示(tips: 可以利用字符串的长度属性 length 以及使用三目运算符)

    function soution(string, limit){
        return string.length>limit?string.substr(0, limit)+'...' : string
    }
    
