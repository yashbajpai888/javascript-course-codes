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
    //it is about functional scope, and ye nearest function tk kahi pr bhi access kia ja skta h.
    ex:-
    function(){
        if(true){
            var a = 12;
        }
        console.log(a);     //yaha tk var 
    }

    constants - is something jo change nahi hota, and variable is something ho change hojata h.

    ex:-  var dulha = "Lab";
        var dulhan = "Labby";
        // here we can change the value in the console
        
    ex:- const 
        var dulha = "Lab";
        const dulhan = "Labby";
        //here we got an error in the console that Uncaught type error.
        //ye bhi ek block scope or ye bhi ek nearest bracket tak hi access kia ja skta ----------
        // lekin iski value hum reinitalize nhi kr skte like 
        ex:- functions(){
            if(true){
                const a = 10;
                a = 20; this cant be done here...
            }
        }

        

// let - let se variables bante h.
    Just like var in Javascript, let keyword is also used for variable declaration. But the only difference is the variable declared with the “let” keyword is block-scoped and local variable. A variable declared with let will be out of scope outside the block within which it has been declared.
    //ye block scope hai or ye sirf nearest brackets tak hi access kia ja skta h.
    ex:-
    function(){
        if(true){   //yaha se 
            let a = 12;
        }   // yaha tak ye access kia ja skta hai.
        console.log(a);     //yaha tak nahi
    }



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
    ex:- to print 0 to 10 numbers.
    for(i = 0; i < 11; i++ )
        start; end;     change
   

    while:- ek aise loop h jo future m jake tutega
    //means ex while continue chalega until the provided condiiton gets false value
    //ex:- while(var i < 20)
    /* toh ye 20 tk print krega mtlb tb tk value true h or 20 aane pr print krna band 
    ho jaega mtlb value false ho jaegi.

    while(condtion) // while lgatar chalta rehta or is condition ko match krta rehta h.
    {

    }
    //means isme aisa h ki while k andar kuch aisa likho jo ki true ho jae, like ex:-
    // while(12>3) here the condition is true that is 12 is greater than 3
    or agr iska answer true aagya toh while kb tk chalega hamesha.

************************************************************************
// Functions - function ka matlab aap kuch code ko likh kr koi naam de sakte ho,
                and bad me usko use kar sakte hai.
                simply function means code ko naam dena.
    functions mainly teen kaam k liye hote h,
        
    1st:- jab aap apna code turant nahi chalana chahte future me chalana chahte ho.
    2nd:- jab aapka code aap reuse krna chahte ho
    3rd:- jab aap code chalana chahte ho har bar with diffrent data

    style there are 6 styles to make funtion in Javascript
    3 are in es5
    3 are in es6
    ex:-
    man lo humne ek code likha bike naam ka.
    bike(){
        ..................................
        ...................................
        ...................................
    }
     toh ab agar hum ko code y code use krna h toh phir s code nhi likhenge
     ab sirf bike likhenge toh y code pura chal jaega.

    
    1st and 2nd ex:- code turant nhi chle bad me chalega, code reuse hoga.
    function hello(){
        console.log("yash");
    }

    3rd example code run every time with diffrent data so for that we'll use 
    params(parameters) and arguments. 
    ex:- we have funtion abcd() or usme bad me while calling  data add hota h 
         or har bar alg data aata hai, or vo bad me add hua vala data arguments kehlata hai
         or vo args jo h parameters me ja kr run hote hai.

    funtion abcd(a) //this a is parameter here.
    {
        console.log(a)
    }
    abcd(12); // this 12 is actually an value or in values ko hum argument kehte h.

    funtion abcd(a,b,c){
        console.log(a,b,c);
    }
    abcd(12,13,14) //this can work like this as well

************************************************************************
    arguments ka matlab hota h real values jo hum dete h functions chalte vakt
    parameters are variables jinme values store hoti h arguments vali
************************************************************************
    arrays 
     variable me ek value store hoti h pr jab multiple values ko store krna ----------
     tab use hota h array ka.

     ex:- 
     var a = [1,2,3]; // here it's an array
************************************************************************
    //push pop shift unshift splice
    //suppose we have made an array 
    var a = [1,2,3,4]

    //"push" array me ek extra member jodne k liye hota h push, ye last m value ko jodta h.
    a.push(5); // this will add an 5 to an existing array

    //"pop" used to remove one member from an array.
    a.pop();

    // "unshift" array me ye front me ek value ko jodta h.
    a.unshift(0);
    
    //"shift" used to remove one value from the front on an array.
    a.shift();

    //"splice" is used to remove one value from an array but isko jis value ko hatana
               hota h uska index dena pdta h or kaha tk hatana h y bhi btana pdta h.

    ex:- suppose we have to remove 3 from the array so we have to give its index number 
         so 3 is on index 2 and we have to remove only 1 element which is 3 so we'll give 1.
    a.splice(2,1);

************************************************************************
    //Objects

    means ek element ya product ki sari values ko store krna in a key value pairs is an Object.
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************
************************************************************************

