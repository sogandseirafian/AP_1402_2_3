# AP_1402_2_3
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace AP_1402_2_9_CS
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //برنامه ای بنویسید که یک عدد 4 رقمی از ورودی دریافت و مجموع ارقام را چاپ کند
            Console.WriteLine("please four digit number:");
            int num = Convert.ToInt32(Console.ReadLine());
            int sum = 0,sdigit;
              while(num>0)
            {
                sdigit= num % 10;
                sum += sdigit;
                num /= 10;
            }
            Console.WriteLine(sum);
        }
    }
}
