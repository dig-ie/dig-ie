# Hello! 🐱

```react
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
      "Software Engineering Analyst",
      "React",
      "TypeScript",
      "REST APIs",
      ".NET",
      "NEST",
      "Dart",
      "FlutterFlow",
    ],
  };

  return <Developer name={devProfile.name} skills={devProfile.skills} />;
};

export default App;
