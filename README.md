# binbin
自我介绍
pragma solidity ^0.4.0;	//向上兼容到0.5.0以下
contract Demo{
    string str = "hello world";
    function getStr() public view returns(string){
        return str;
    }
    function setStr(string  t_str) public{
        str = t_str;
    }
    function pureTest(string t_str) public  pure returns(string){
        return t_str;
    }
}
    bytes arr = new bytes(2);
    function setArr() public{
        arr[0]=0x01;   arr[1]=0x02;
    }
    function getArr() public view returns(uint){
        return arr.length;
    } 
    function pushData() public {
        //arr.length = 3;
        arr.push(0x03);
    }
	string str="hello world";
    function getLength() public view returns (uint){
        return bytes(str).length;
    }
    function getStr() public view returns (bytes){
        return bytes(str);
    }
    function getChar() public view returns (bytes1){
        return bytes(str)[0];
    }
    function opChar() public {
        bytes(str)[0] = 'x';
    }
