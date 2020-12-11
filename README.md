// Submission-for-micheal-reeves-discord-
//this is c# btw
//quick bruteforce alg cuz all my other projects are personal


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;


namespace Bruteforce_Alg
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Password: ");
            string password = Console.ReadLine();
            string attempt = "";

            int first = 0;
            int second = 0;
            int third = 0;
            int fourth = 0;
            int fifth = 0;
            int sixth = 0;
            int seventh = 0;
            int eighth = 0;


            int cracks = 0;

            string[] array = new string[63];
            array[0] = "";
            array[1] = "a";
            array[2] = "b";
            array[3] = "c";
            array[4] = "d";
            array[5] = "e";
            array[6] = "f";
            array[7] = "g";
            array[8] = "h";
            array[9] = "i";
            array[10] = "j";
            array[11] = "k";
            array[12] = "l";
            array[13] = "m";
            array[14] = "n";
            array[15] = "o";
            array[16] = "p";
            array[17] = "q";
            array[18] = "r";
            array[19] = "s";
            array[20] = "t";
            array[21] = "u";
            array[22] = "v";
            array[23] = "w";
            array[24] = "x";
            array[25] = "y";
            array[26] = "z";
            array[27] = "A";
            array[28] = "B";
            array[29] = "C";
            array[30] = "D";
            array[31] = "E";
            array[32] = "F";
            array[33] = "G";
            array[34] = "H";
            array[35] = "I";
            array[36] = "J";
            array[37] = "K";
            array[38] = "L";
            array[39] = "M";
            array[40] = "N";
            array[41] = "O";
            array[42] = "P";
            array[43] = "Q";
            array[44] = "R";
            array[45] = "S";
            array[46] = "T";
            array[47] = "U";
            array[48] = "V";
            array[49] = "W";
            array[50] = "X";
            array[51] = "Y";
            array[52] = "Z";
            array[53] = "0";
            array[54] = "1";
            array[55] = "2";
            array[56] = "3";
            array[57] = "4";
            array[58] = "5";
            array[59] = "6";
            array[60] = "7";
            array[61] = "8";
            array[62] = "9";

            while (!attempt.Equals(password))
            {
                if (first == array.Length)
                {
                    second++;
                    first = 0;
                }
                if (second == array.Length)
                {
                    third++;
                    second = 0;
                }
                if (third == array.Length)
                {
                    fourth++;
                    third = 0;
                }
                if (fourth == array.Length)
                {
                    fifth++;
                    fourth = 0;
                }
                if (fifth == array.Length)
                {
                    sixth++;
                    fifth = 0;
                }
                if (sixth == array.Length)
                {
                    seventh++;
                    sixth = 0;
                }
                if (seventh == array.Length)
                {
                    fourth++;
                    seventh = 0;
                }
                if (eighth == array.Length)
                {
                    break;
                }

                attempt = array[eighth] + array[seventh] + array[sixth] + array[fifth] + array[fourth] + array[third] + array[second] + array[first];

                Console.WriteLine(attempt);
                first++;
                cracks++;
            }
            Console.WriteLine("> Attempts to crack: " + cracks);

        }
    }
}
