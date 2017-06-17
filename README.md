using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Exam_1
{
    class Program
    {
        static void Main(string[] args)
        {
            double x = double.Parse(Console.ReadLine());
            double y = double.Parse(Console.ReadLine());
            double h = double.Parse(Console.ReadLine());

            double side = ((x * y) * 2) - ((1.5 * 1.5) * 2);
            double backFron = ((x * x) * 2) - (1.2 * 2);

            double houseArea = side + backFron;
            houseArea /= 3.4;

            double roof = ((x * y) * 2) + (((x * h) / 2) * 2);
            roof /= 4.3;

            Console.WriteLine("{0:f2}", houseArea);
            Console.WriteLine("{0:f2}", roof);
        }
    }
}
