# js
qch4
document.getElementById('myForm').addEventListener("submit", function (e) {
    let toPay;
    let given;
    let toGive;
    let nb10;
    let nb5;
   let nb1;

let msg10 = document.getElementById("10").value;
let msg5 = document.getElementById("5").value;
let msg1 = document.getElementById("1").value

msg10.innerHTML = "0";
msg5.innerHTML = "0";
msg1.innerHTML = "0";


    toPay = document.getElementById("total").value;
    given = document.getElementById("given").value;
    
    toGive = given - toPay;
    nb10 = 0;
    while(toGive >=10){
        nb10 = nb10 +1;
        toGive = toGive -10;
    }
nb5 =0;
while(toGive >=5){
    nb5 = nb5 +1;
    toGive = toGive -5;
}
nb1 =0;
while(toGive >=1){
    nb1 = nb1 +1;
    toGive = toGive-1;
}
msg10.innerHTML = nb10;
msg5.innerHTML = nb5;
msg1.innerHTML = nb1;
/*toGive = nb10 +" "+ 'billets de 10' +" "+"et"+" "+ nb5 +" "+ 'billets de 5' +" "+"et"+" "+nb1 +" "+ 'pièces de 1 vous sera rendu';
alert(toGive);*/

})
