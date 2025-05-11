using System;

namespace ProjeAdi
{
    internal class Program
    {
        static void Main(string[] args)

        {
            // Kodlar buraya yazılır

            Console.WriteLine("Rüya Manavına hoşgeldiniz!");
            Console.WriteLine("\nFiyat Listesi:");
            Console.WriteLine("Elma = 2 TL");
            Console.WriteLine("Armut = 3 TL");
            Console.WriteLine("Çilek = 2 TL");
            Console.WriteLine("Muz = 3 TL");
            Console.WriteLine("Diğer bütün meyveler = 4 TL");
            Console.WriteLine(); // boş satır

            Console.Write("Hangi meyveyi satın almak istersiniz? (Elma/Armut/Çilek/Muz/Diğer): ");
            string secilenMeyve = Console.ReadLine()!;
            string fiyat;

            switch (secilenMeyve.ToLower())
            {
                case "elma":
                    fiyat = "2 TL";
                    break;
                case "armut":
                    fiyat = "3 TL";
                    break;
                case "çilek":
                    fiyat = "2 TL";
                    break;
                case "muz":
                    fiyat = "3 TL";
                    break;
                default:
                    fiyat = "4 TL";
                    break;
            }

            Console.WriteLine("Seçtiğiniz meyvenin fiyatı : " + fiyat);
        }
    }
}
        
    // Bu ödevi If-else ile de yaptım ama if else projesini nereye cohort a yüklemedim ama Github tan bakabilirsiniz. 
    // Bu projenin Switch Case ile yazılması daha doğru. Çünkü if-else de her if ayrı bir koşul olduğu için proje uzuyor.
    // Ayrıca, Switch Case daha hızlı çalışıyor. If else de her koşulu ayrı ayrı deniyor ama switch case de öyle değil şartları uygun olanı seçiyor ve devam ediyor.
