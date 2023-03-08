Функция с именем getA(b) имеет объект b.bye со значением 'teacher', и вызов getA(a) приведет к тому, что a будет равно {bye = 'teacher'}. При использовании console.log(a) аутпут первой функции будет равен:
{bye: 'teacher'}.

const a = {};
function getA(b) {
    b.bye= 'teacher'
};

getA(a)
console.log(a);


Функция с именем getA(b) имеет b со значением 'null', но так как b никак не влияет на значение обьекта, он не будет учтён при вызове getA(a). При использовании console.log(a) результатом первой функции будет равен const a: 
{hello: 'student'}.

const a = {hello: 'student'};
function getA(b) {
    b = null
};
getA(a)
console.log(a);