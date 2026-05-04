using System;
namespace ArrayApp
{
class Block1
{
   
    static void RemoveByValue(ref int[] a, int key)
    {
        if (a.Length == 0)
        {
            Console.WriteLine("Масив порожній");
            return;
        }

        int pos = -1;

        for (int i = 0; i < a.Length; i++)
        {
            if (a[i] == key)
            {
                pos = i;
                break;
            }
        }

        if (pos == -1)
        {
            Console.WriteLine("Такого елемента нема");
            return;
        }

        int[] b = new int[a.Length - 1];

        for (int i = 0; i < pos; i++)
            b[i] = a[i];

        for (int i = pos + 1; i < a.Length; i++)
            b[i - 1] = a[i];

        a = b;
    }

    static void Main()
    {
       int[] arr = { 5, 3, -1, 7, 3, 0 };
            int key = 3;
            RemoveByValue(ref arr, key);
            foreach (int x in arr)
                Console.Write(x + " ");
    }
}
}
