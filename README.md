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
    "skills": [
  "Full Stack Developer",
  "React",
  "React Native",
  "FlutterFlow",
  "TypeScript",
  "REST APIs",
  "GraphQL",
  "Node.js",
  "NestJS",
  ".NET",
  "Git",
  "GitHub",
  "Dart",
  "PostgreSQL",
  "MySQL",
  "NoSQL (MongoDB, MongoDB Atlas, Redis)",
  "AWS (Lambda, S3, DynamoDB)",
  "GCP",
  "Supabase",
  "Docker",
  "CI/CD (GitHub Actions, Vercel)"
],
  };

  return <Developer name={devProfile.name} skills={devProfile.skills} />;
};

export default App;
```
