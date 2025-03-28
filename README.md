# Hello! 🐱

```tsx
import React from "react";

interface DeveloperProps {
  name: string;
  skills: string[];
}

const Developer: React.FC<DeveloperProps> = ({ name, skills }) => {
  return (
    <div style={{ padding: "20px", fontFamily: "Arial" }}>
      <h2>Name: {name}</h2>
      <p>Skills: {skills.join(", ")}</p>
    </div>
  );
};

const App: React.FC = () => {
  const devProfile = {
    name: "Diêgo de Barros",
    skills: [
      "Full stack developer",
      "React",
      "FlutterFlow"
      "TypeScript",
      "REST APIs",
      "Node.js",
      ".NET",
      "Git",
      "NEST",
      "Dart",
      "SQL",
      "Postgres",
      "noSQL (mongodb e mongodb atlas)"
    ],
  };

  return <Developer name={devProfile.name} skills={devProfile.skills} />;
};

export default App;
```
