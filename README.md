# Triangle

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Triangle
{
    public static class TriangleSolver
    {
        public static string Analyze(int a, int b, int c)
        {
            string result = string.Empty;
            if (((a + b) > c) && ((b + c) > a) && ((c + a) > b))
            {
                Console.WriteLine("It's a triangle(because sum of two side should be greater than third side)");

                if (a == b && b == c && a == c)
                {
                    result = "It's an Equilateral triangle";

                }
                else if (a == b || b == c || a == c)
                {
                    result = "It's an Isosceles triangle";

                }
                else
                {
                    result = "It's a Scalene triangle";

                }


            }
                else
                {
                    result="It's not a valid triangle";
                }
           return (result);
            }
        }
    } 
