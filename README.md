# zada4a
using System;

namespace _09.spiceMustFlow
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int startingYield = int.Parse(Console.ReadLine());
            int daysCount = 0;
            int spiceVolume = 0;
            int forCrew = 26;


            while (startingYield >= 100)
            {
                spiceVolume += startingYield - forCrew;
                startingYield -= 10;
                daysCount++;             
            }
            if (spiceVolume >= 26)
            {
                spiceVolume -= forCrew;
            }
            Console.WriteLine(daysCount);
            Console.WriteLine(spiceVolume);
        }
    }
}
