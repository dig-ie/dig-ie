# Hello! 🐱‍👤🔧💻

```csharp
using System;
using System.Collections.Generic;

class Developer
{
    public string Name { get; }
    public List<string> Skills { get; }

    public Developer(string name, List<string> skills)
    {
        Name = name;
        Skills = skills;
    }

    public void GetDeveloperInfo()
    {
        Console.WriteLine($@"
            Name: {Name}
            Skills: {string.Join(", ", Skills)}
        ");
    }
}

class Program
{
    static void Main()
    {
        var devProfile = new Developer(
            "Diêgo de Barros",
            new List<string>
            {
                "Software Engineering Analyst",
                "React",
                "TypeScript",
                "REST APIs",
                ".NET",
                "NEST",
                "Dart",
                "FlutterFlow"
            }
        );

        devProfile.GetDeveloperInfo();
    }
}
