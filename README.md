# multiple-inheritance
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace simpleinheritance
{
    public class student
    {
        public void showinfo()
        {
            Console.WriteLine("Name:Snehal");
        }
    }
    interface exam
    {
        void subinfo();
    }
    class result:student,exam
    {
        public void subinfo()
        {
            Console.WriteLine("subject:c#.net");
        }
        static void Main(string[] args)
        {
            result obj = new result();
            obj.showinfo();
            obj.subinfo();
            Console.ReadLine();
        }
         
    }
}
