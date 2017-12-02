# thing
help
using System;

namespace Goodluck
{
	class MainClass
	{
		public static void Main (string[] args)
		{
			Random g = new Random ();
			int num;
			num = g.Next (1, 11);
			Console.WriteLine ("Guess the number from 1 to 10");
			int i = 0;
			do {
				Console.WriteLine ("Enter number");
				try
				{
				i = Convert.ToInt32(Console.ReadLine ());
				}
				catch (Exception)
				{
					Console.WriteLine ("Error");
				}
				finally
				{
				Console.Clear ();
				}
			} while (i != num);    
			Console.Clear ();
				Console.WriteLine (num);
		} 
	} 
} 
