1. While loop
While Loop में कोड तब तक लगातार execute होते रहता है जब तक कि एक condition सत्य(true) नहीं हो जाती है. यह सबसे पहले condition की जांच करता है और बाद में code को execute करता है.
while Loop का प्रयोग करते समय निम्न बिन्दुओं का ध्यान रखा जाना चाहिए. while लूप को हमेशा कीवर्ड while से स्टार्ट किया जाता है एवं उसके अंदर कंडीशन को ब्रैकेट () में लिखा जाता है, जैसे while (count < 10) while लूप कीवर्ड एवं कंडीशन के बाद लूप की बॉडी स्टेटमेंट को कर्ली ब्रेसेस { } के अंदर लिखा जाता है, जैसे

while loop में 3 steps हम अलग अलग लिखते हे।
while (condition){  
    // code 
}  
Example for While Loop
var i = 0;
while(i<10){
	document.write("i + "<br />");
	i++;
}
Nested While Loop Example
JavaScript में Nested While Loop का भी use कर सकते हैं , मतलब While Loop के अंदर एक और While Loop ले सकते हे 
let a  = 1;
     while(a <= 20){
       let b = 1;
       document.write(b+ " ");
       while(b < a){
         b++;
         document.write(b+" ");
       }
       ++a;
       document.write("<br>");
     }
 



2. Do while
do_while Loop जब तक condition true होती है तब तक statements को बार-बार executes करता रहता है और जब condition false हो जाती तब एक बार statement को execute करता है |
do while loop में 3 steps हम अलग अलग लिखते हे।


do{
	//do Statement(s);
}while(condition);
Example for While Loop
var i = 0;
do{
	document.write("i + "<br />"); ");
	i++;
}while(i<10);
3. For Loop 
For Loop में दिए हुए number तक statements repeat होते रहता है |
Syntax for 'For' Loop
फ़ोर लॊप को हम एक साथ लिखते है


for(initialization; condition; increment/decrement){
	//for Statement(s);
intialization : यहाँ पर variable को initialize करना पड़ता | यहाँ पर जो value दी जाती है वही से loop start हो जाता है |
condition : यहाँ पर condition होती है , जब तक condition true होती है तब तक loop iterate होता रहता है और बाद में loop का contrl बाहर आकर iteration stop हो जाता है |
increment/decrement : यहाँ पर value को increase या decrease की जाती है |
for(var i=0;  i<10;  i++){
	document.write(i + "<br />");
}
2. For In Loop
For..in Loop से Object की हर एक property को iterate किया जाता है |
for(variable in object){
	//statements;
}
variable : यहाँ पर object की properties को iterate करने के लिए variable लिया जाता है |
object : यहाँ पर जिस Object की properties को iterate करना है उस object का नाम आता है |
var arr = [1, 2, 3, 4]; 
for (var element in arr) {
  document.write("index[" + element + "] = " + arr[element] + "<br />");
}


Output :
index[0] = 1
index[1] = 2
index[2] = 3
index[3] = 4
2. For of Loop
और for loop की तुलना में for of loop काफी easy to understand और weaknesses को improve किया है , by eliminating the counting logic and exit condition.
JavaScript for of Loop Syntax
for(val of object)
{
  //write your logic here
}


JavaScript for of Loop Example
Iterating over a string.
  /* defining JavaScript String Object */
      let object = new  ("Welcome");
      for(val of object){  
        document.write(`value : ${val}<br>`);
      }


