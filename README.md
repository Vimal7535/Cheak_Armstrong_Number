# Cheak_Armstrong_Number


using System;

namespace Cheak_Armstrong_Number

{
    class Program
    {
        static void Main(string[] args)
        {
            int cube;
            int result = 0 ;
            int rem;
            int temp;
            
            Console.WriteLine("Enter the Number:");
            int num = int.Parse(Console.ReadLine());
            temp = num;                
                while(num!=0)
                {
                    rem = num % 10;
                    cube = rem * rem * rem;
                    result = result + cube;
                    num = num / 10;
                }           
            if(temp==result)
            {
                Console.WriteLine("Armstrong NUmber");
            }
            else
            {
                Console.WriteLine("Not Armstrong Number.");
            }

        }
    }
}
