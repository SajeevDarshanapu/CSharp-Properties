# CSharp-Properties

1)We can access private variables using properties
2)It has two methods
         i)Get
         ii) Set
3)The Get methods "returns" the value of a variable name 
4) The Get method represents a value returning method without parameter 
-------------------- 
5) The Set method "assigns" a value to the variable name
6) The Set method represents a non value returning method with parameter
--------------------
7)Combining the two methods(Get and Set) together making it in a simple form called as Property
8)Property is a member of a class using which we can expose the values associated with the class to the outside environment

--------------------
class Sajeev
{
    private string name;
    public string Name
    {
        get
        {
            return name;
        }
        set
        {
            name=value;
        }
    }
    class Nani
    {
         public static void Main ()
        {
            Sajeev Obj = new Sajeev();
            Obj.Name="HeadBanger";                        //output: HeadBanger
            Console.WriteLine(Obj.Name);
        }
    }
}

# Automatic Properties(SHORT HAND)

1) We don't have to define the field for the property
2) We only have to write get; and set;


   class Sajeev
   {
   public string Name
   {get;set;}
   }
   class Nani
   {
         public static void Main ()
        {
            Sajeev Obj = new Sajeev();
            Obj.Name="HeadBanger";                        //output: HeadBanger
            Console.WriteLine(Obj.Name);
        }
    }
        
   ------------------------------
   
   # Encapsulation
   
   1)Better control of class memebers(Reduces the probability of messing up the code)
   2)Fields can be made read only( If we only used get method)
   3)Fields can be made write only(If we only used set method)
   4)Increased security of data
   5)Flexible: The programmer can change one part of code without affecting the other parts
