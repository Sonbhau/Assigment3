# Assigment3
# Que1
class Arithematic
{
    
    No1 : number
    No2 : number
    constructor(A:number,B:number)
    {
        this.No1 = A
        this.No2 = B


    }
    Addition():number
{
        return this.No1+this.No2
    }

    Substraction():number
    {
        return this.No1-this.No2
    }
    Multiplication():number
    {
        return this.No1 *this.No2
    }
    Division():number
    {
        return this.No1 / this.No2
    }
}

var obj1 = new Arithematic(49,35)

var Ret : number = 0
Ret = obj1.Addition()
console.log("Addition of obj1:"+Ret)

Ret = obj1.Substraction()
console.log("Substraction of obj1:"+Ret)

Ret = obj1.Multiplication()
console.log("Multiplication of obj1:"+Ret)

Ret = obj1.Division()
console.log("Division of obj1:"+Ret)


#Que2

class Circle
{
  Radius : number
  PI : number

  constructor(Data : number)
  {
    this.Radius = Data 
    this.PI  = 3.14
  }
   
  CalculateArea():number
  {
    let Ans : number = 0

    Ans = this.PI *this.Radius*this.Radius
    return Ans
  }
}

var obj = new Circle(9.3)

var Ret : number = 0

Ret = obj.CalculateArea()

console.log("Area is :"+Ret)

#Que3

class Circle
{
    Radius : number;
    PI : number;

    constructor(Data : number)
    {
        this.Radius = Data;
        this.PI = 3.14; 
    }

    CalculateArea() : number
    {
        let Ans : number = 0;
        Ans = this.PI * this.Radius * this.Radius;
        return Ans;
    }

}

class CircleX extends Circle
{
    constructor(Value : number)
    {
        super(Value);
    }

    Circumfarance()
    {
        return 2 * this.PI * this.Radius;
    }
}

var obj1 = new CircleX(9.3);
var Ret : number = 0;

Ret = obj1.CalculateArea();
console.log("Area of circle1 is : "+Ret);

Ret = obj1.Circumfarance();
console.log("Circumfarance of circle1 is : "+Ret);

console.log();

var obj2 = new CircleX(13.4);

Ret = obj2.CalculateArea();
console.log("Area of circle2 is : "+Ret);

Ret = obj2.Circumfarance();
console.log("Circumfarance of circle2 is : "+Ret);
