# parcial-estructura
biblioteca

using System;
using System.Linq; 
using System.Text;

class libro
{
    private string titulo, coleccion, autor;
    private int codigo, paginas;

    public libro(int codigo, string titulo, string coleccion, string autor, int paginas)
    {
        setCodigo(codigo);
        setTitulo(titulo);
        setColeccion(coleccion);
        setAutor(autor);
        setPaginas(paginas);

    }
    public void setCodigo(int n) { codigo = n; }
    public void setTitulo(string a) { titulo = a; }
    public void setColeccion(string d) { coleccion = d; }
    public void setAutor(string s) { autor = s; }
    public void setPaginas(int f) { paginas = f; }

    public int getCodigo() { return codigo; }
    public string getTitulo() { return titulo; }
    public string getColeccion() { return coleccion; }
    public string getAutor() { return autor; }
    public int getPaginas() { return paginas; }

    public void mostrarlibro()
    {
        Console.Write("\nCodigo:" + getCodigo() + "\nTitulo:" + getTitulo() + "\nColeccion:" + getColeccion() + "\nAutor:" + getAutor() + "\nPaginas" + getPaginas());
    }
}
public class Principal
{
    public static void main()
    {
        string titulo, coleccion, autor;

        int codigo, pagina;

        Console.Write("por favor ingresar codigo del libro: ");
        codigo = int.Parse(Console.ReadLine());

        Console.Write("por favor ingresar titulo del libro:");
        titulo = Console.ReadLine();
        
        Console.Write("por favor ingresar coleccion: ");
        coleccion = (Console.ReadLine());

        Console.Write("por favor ingresar autor del libro:");
        autor = (Console.ReadLine());

        Console.Write("por favor ingresar cantidad de pagina:");
        pagina = int.Parse(Console.ReadLine());
              
        libro 1;
        1 = new libro(codigo, titulo, coleccion, autor, pagina);
        1.mostrarlibro();
         
    } 
}

