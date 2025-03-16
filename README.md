type Dev = { name: string; skills: string[] };
class DeveloperProfile {
    constructor(private readonly developer: Dev) { }
    getDeveloperInfo() {
        console.log(`
            Name: ${this.developer.name}
            Skills: ${this.developer.skills.join(", ")}`
        )
    }
}
const devProfile = new DeveloperProfile({
    name: "Diêgo de Barros",
    skills: [
        "Software Engineering Analyst",
        "React",
        "TypeScript",
        "REST APIs",
        ".NET",
        "NEST",
        "Dart",
        "FlutterFlow",
    ]
});
devProfile.getDeveloperInfo();
