# Expression body in C#

Expression body definitions let you provide a member's implementation in a **very concise, readable form.**
It supports in over C# 6.0, expecially memeber of Constructor is supported in C# 7.0

It has the following general syntax:
> member => expression;

### Constructor ###
- definition for a constructor typically consists of a single assignment expression 
- a method call that handles the constructor's arguments or initializes instance state

```
public class Location
{
   private string locationName;
   
   public Location(string name) => Name = name;

   public string Name
   {
      get => locationName;
      set => locationName = value;
   } 
}
```

