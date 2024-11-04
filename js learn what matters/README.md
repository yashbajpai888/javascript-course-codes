// word vs keyword
 word - the thing which doesn't have any meaning is word.
  is that jiska js me koi matlab nhi hota like 
 chacha or chachi = xyz 
 
 keyword - the thing which has some meaning is keyword.
    is that which is predefined or already known to js like 
    for // its an loop

************************************************************************
//undefined -
    means whose value is not defined ex:-
    means hamare pass koi chiz h, but uski value nhi pta. 
    var a;
    console.log(a);
    //isme yha hame a ek variable h y toh pta h pr uski value koi defined nahi h.

// not-defined 
    means vo chiz define hi nhi ki h.
    like we defined ex:-
    var a = 12; // but calling b
    console.log(b); //then it will give an undefined error.

************************************************************************
// declaration and initialzation
    var a; //declaration
    a = 10; // initialization
    
************************************************************************
// var const let


// variables and constants 
    variables - code me koi bhi data store karne ke liye jiska use hota h, use kehte h, variable.

    constants - is something jo change nahi hota, and variable is something ho change hojata h.

    ex:-  var dulha = "Lab";
        var dulhan = "Labby";
        // here we can change the value in the console
        
    ex:- const 
        var dulha = "Lab";
        var dulhan = "Labby";
        //here we got an error in the console that Uncaught type error.

// let - let se variables bante h.


************************************************************************
//Hoisting
 Hoisting - variable ko banane se phle usse use kr skte h.
 variables and functions are hoisted which means their declaration is moved on the top of code.

 ex:- we have made an variable num3 = 10;
      on line 5 but we use console.log(num3); in line 4 so we can use it in js not in other language.




************************************************************************
//Types in js
    has 2 types primitives and references   -- bracket nahi h value me matlb primitive value h, bracket h matlab reference type ki value h.
    primitives - number, string, null, undefined, boolean.
    references - [] () {}

// aisi koi bhi value jisko copy karne par real copy nahi hota, balki us main value ka reference pass hojata h,
    use hum reference value kehte h, 
    or jiska copy krne pr real copy ho jae wo value primitive type value hoti h.

    primitive ex:-
    var a = 10;
    var b = a; // this is an primitive value

    reference ex:-
    var a = [1,2,3,4];

    like 
    var a = 10;
    var b = a;
    b.pop();

Note:- [] {}  () this are brackets values, we cannot directly copy this value, we can copy but not directly copy, 
    we cannot do this directly
    //yaha a k pass h khud ka 1 2 3 4 or b k pass h a ka 1234 so if we perform some changes in b it will automatically be performed on a.

    var a = [1,2,3,4]
    var b = a;
    b.pop();
    //will give 123 as an op
    
************************************************************************
// Conditionals - if else else-if 

    **jab bhi bat agar magar pr aaegi, ya aise vaise pr aegi ya, aisa hua toh vo karo vaisa hua toh vo karo pr aaegi. 
************************************************************************
// loops - for while

    loop ka matlab repeat ex:-
    // 1 2 3 4 5 6 7 8 9
    // 1 1 1 1 1 1 1 1 1 
    here both are loops  

    for(start;end;change){

    }

    while:- ek aise loop h jo future m jake tutega

    while(condtion) // while lgatar chalta rehta or is condition ko match krta rehta h.
    {

    }

************************************************************************
// Functions 
    function ka matlab aap kuch code ko likh kr koi naam de sakte ho.
    functions mainly teen kaam k liye hote h,
    1st:- jab aap apna code turant nahi chalana chahte future me chalana chahte ho.
    2nd:- jab aapka code aap reuse krna chahte ho
    3rd:- jab aap code chalana chahte ho har bar with diffrent data

    ex:-
    function hellobolo(){
        console.log("hello");
    }
    hellobolo();

************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************

