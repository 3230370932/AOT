pragma solidity ^0.4.24;


contract Chain{

   uint ethWei = 1 ether;
    
   address owner;
    
   event Instructor(address _address,uint _amount,uint _type,string  _usernumber); 
    
   function invest(uint inputAmount,string memory  beInvitedCode,uint _amount) public payable{
   
          address _useraddress=msg.sender;
          
          inputAmount =  msg.value;
          
          emit Instructor(_useraddress,inputAmount,0,beInvitedCode);
         
    }

}
