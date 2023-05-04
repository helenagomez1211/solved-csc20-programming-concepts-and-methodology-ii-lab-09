Download Link: https://assignmentchef.com/product/solved-csc20-programming-concepts-and-methodology-ii-lab-09
<br>
Objective: This assignment will give you practice with action event handling.

The programming assignment:

In this assignment you are to add functionality to the calculator created in lab 08. You don’t have to make the calculator a full function calculator. You only need to make buttons 0 ~ 9, +, -, *, / and = work.




Some programming hints:




<ol>

 <li>Implement an action listener.</li>

</ol>




public void actionPerformed(ActionEvent e) {  for (int i=0; i&lt;=9; ++i) {                    if (e.getSource() == digitButton[i]) {

if (newNumber) {

display digit in tf;

newNUmber = false;

} else append digit in tf;

return;

}

}

if (e.getSource() == addButton ){      opnd1 = Double.parseDouble(tf.getText());

newNumber = true;

operator = ‘+’; return;

}

if (e.getSource() == eqButton) {                      opnd2 = Double.parseDouble(tf.getText());                               switch (operator) {                                           case ‘/’: res = opnd1 / opnd2; break;                                       case ‘*’: res = opnd1 * opnd2; break;                                       case ‘-‘: res = opnd1 – opnd2; break;

case ‘+’: res = opnd1 + opnd2; break;

}

display(“”+res);    newNumber = true;               return;

}

}




<ol start="2">

 <li>Register the action listener with all buttons.</li>

</ol>





