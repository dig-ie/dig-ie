# Hello!

using System;

class Developer
{
    public string Name { get; }
    public string[] Skills { get; }

    public Developer(string name, params string[] skills)
    {
        Name = name;
        Skills = skills;
    }

    public void ShowProfile()
    {
        Console.WriteLine($"👨‍💻 {Name}\n🔹 Skills: {string.Join(", ", Skills)}");
    }
}

class Program
{
    static void Main()
    {
        new Developer("Diêgo de Barros", 
            "Software Engineering Analyst", "React", "TypeScript", 
            "REST APIs", ".NET", "NEST", "Dart", "FlutterFlow"
        ).ShowProfile();
    }
}

