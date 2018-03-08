
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp330
{
    class Program
    {
        static void Main(string[] args)
        {
            Dictionary<string, string> users = new Dictionary<string, string>();
            string line;
            while ((line = Console.ReadLine() )!= "stop")
            {
                string name = line;
                string email = Console.ReadLine();
                if (email.EndsWith("us") || email.EndsWith("uk"))
                {
                    continue;
                }
                if (!users.ContainsKey(name))
                {
                    users.Add(name, email);
                }
                else
                {
                    users[name] = email;
                }
            }
            foreach (var user in users)
            {
                Console.WriteLine($"{user.Key}->{user.Value}");
            }
        }
    }
}


