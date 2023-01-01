```c#
//needs to be seperated before executed

/////////
int i = 0;  //zero is included. start from -1 to exclude it
int s = 1;
while (s != 0){
    s = Convert.ToInt32(Console.ReadLine());
    i++;
}
Console.WriteLine(i);

/////////
int n = 0;
int s = 0;
do{
    s = Convert.ToInt32(Console.ReadLine());
    n += s;
} while (s != 0);
Console.WriteLine(n);


/////////
int n = 0;  
int s = 0;
float i = 0;    
do{
    s = Convert.ToInt32(Console.ReadLine());
    n += s;
    i++;    //also counts 0. so exclude it while averaging (i-1)
} while (s != 0);
Console.WriteLine(n / (i-1));   //possible dividing by zero error


/////////
int s = Convert.ToInt32(Console.ReadLine());
bool isPrime = true;
for (int i = 2; i < s; i++){   //assumes the number is bigger than 2
    isPrime = !(s % i == 0);
    if (!isPrime){
        break;
    }
}
if (isPrime){
    Console.WriteLine("Prime");
}else{
    Console.WriteLine("not prime");
}



////////
int n = Convert.ToInt32(Console.ReadLine());
if (n % 2 != 0){
    n--;
}
for (int i = n+2; i <= n + 20; i +=2){
    Console.WriteLine(i);
}


////////
int a = Convert.ToInt32(Console.ReadLine());
int b = Convert.ToInt32(Console.ReadLine());
Console.WriteLine(a / b);
Console.WriteLine(a % b);

```
