# VALORES-COMPUESTOS

1. ESTRUCTURA.

using System;

namespace Estructura_Referencia_Clase
{
    
    class Program
    {
        struct datosPersonales
        {
            public string nombreCompleto;
            public int edad;
            public string númeroCédula;
            public string númeroTelefónico;
        }

        public static void Main()
        {
            datosPersonales persona1 = new datosPersonales();
            persona1.nombreCompleto = "David Cardona Franco";
            persona1.edad = 19;
            persona1.númeroCédula = "1002653810";
            persona1.númeroTelefónico = "3127910887";

            Console.WriteLine("Me llamo {0} y tengo {1} años, número de cédula: {2} y número telefónico: {3}", persona1.nombreCompleto, persona1.edad, persona1.númeroCédula, persona1.númeroTelefónico);

        }
    }
}

-------------------------------------------------------------------------------------

2. CLASE.

using System;

namespace Estructura_Referencia_Clase
{
    class Program
    {
        static void Main(string[] args)
        {
            Círculo nuevoCírculo = new Círculo();
            Console.WriteLine("El área del círculo es de: " + nuevoCírculo.calcularÁrea(5.1));
        }
    }

    public class Círculo
    {
        static double pi = 3.1415;
        public double calcularÁrea (double radio)
        {
            return (pi * Math.Pow(radio, 2));
        }
    }
}

