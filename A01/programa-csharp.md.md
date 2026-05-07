# Programa en C# per calcular la lletra del DNI  
  
## Introducció  
  
En aquesta activitat he creat un programa en C# utilitzant Visual Studio Code.  
  
L’objectiu del programa és calcular automàticament la lletra d’un DNI introduint només el número.
---  
  
## Instal·lació de l’entorn  
  
Primer vaig instal·lar:  
  
- Visual Studio Code  
- Extensió de C# per VSCode  
  
---  
  
## Codi font  
  
Aquest és el codi que he creat:  
  
```csharp  
using System;  
  
class Program  
{  
static void Main()  
{  
string[] lletres = {  
"T", "R", "W", "A", "G", "M", "Y", "F",  
"P", "D", "X", "B", "N", "J", "Z", "S",  
"Q", "V", "H", "L", "C", "K", "E"  
};  
  
Console.Write("Introdueix el número del DNI (sense lletra): ");  
int numeroDNI = Convert.ToInt32(Console.ReadLine());  
  
int residu = numeroDNI % 23;  
  
string lletra = lletres[residu];  
  
Console.WriteLine("La lletra del DNI és: " + lletra);  
  
Console.WriteLine("DNI complet: " + numeroDNI + lletra);  
}  
}  
```  
  
---  
  
## Explicació del funcionament  
  
El programa funciona així:  
1. L’usuari introdueix el número del DNI.  
2. El programa calcula el residu entre 23.  
3. Busca la lletra corresponent dins un array.  
4. Mostra el DNI complet.  
  
---  
  
## Exemple d’execució 1  
  
```text  
Introdueix el número del DNI (sense lletra): 12345678  
La lletra del DNI és: Z  
DNI complet: 12345678Z  
```  
  
---  
  
## Exemple d’execució 2  
  
```text  
Introdueix el número del DNI (sense lletra): 11111111  
La lletra del DNI és: H  
DNI complet: 11111111H  
```  
---  
  
## Vídeo de Google Vids  
  
Aquí incrustaré el vídeo explicatiu creat amb Google Vids.  
  
(https://drive.google.com/file/d/1C5RYqo2fbSVWfT3qQwJ1bjUGwlrYMJo1/view?usp=sharing))