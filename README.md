# tester
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp166
{
    class Program
    {
        static void Main(string[] args)
        {
            List<int> numbers = Console.ReadLine().Split(' ').Select(int.Parse).ToList();
            int position = int.Parse(Console.ReadLine());
            var helper = numbers.Skip(position).ToList();
            for (int i = 0; i < position; i++)
            {
                helper.Add(numbers[i]);
            }
            numbers = helper;
            Console.WriteLine(string.Join(" ",numbers));
        }
    }

