[Welocome to my profile!](https://github.com/abbZe/profile-images/blob/main/welcome.png?raw=true)

![TypeScript](https://badges.frapsoft.com/typescript/love/typescript.svg?v=101)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=abbZe.abbZe)

```typescript
interface IFullstackDev {
    name: string;
    role: string;
    languages: string[];
    greetings: () => string;
}

interface IFullstackDevOpts {
    name: string;
    role: string;
    languages: string[];
}

class FullstackDev implements IFullstackDev {
    name: string;
    role: string;
    languages: string[];

    constructor({ name, role, languages }: IFullstackDevOpts) {
        this.name = name;
        this.role = role;
        this.languages = languages;
    }

    greetings() {
        return `Благодарю за посещение профиля ${this.name},
                надеюсь вы нашли что-то интересное для себя :)`;
    }
}

const dimaOpts: IFullstackDevOpts = {
    name: 'Dmitrii',
    role: 'Fullstack Dev',
    languages: ['ru_RU', 'en_US'],
};

const fullStackDevDima = new FullstackDev(dimaOpts);

console.log(fullStackDevDima.greetings());
```

# My library

| Book                                           | Author                       | Category |
|------------------------------------------------|------------------------------|----------|
| Clean Code                                     | Robert Martin                | Common   |
| Clean Architecture                             | Robert Martin                | Common   |
| Code Complete                                  | Steve McConnel               | Common   |
| Extreme Programming                            | Kent Beck                    | Common   |
| JavaScript Patterns                            | Stoyan Stefanov              | Common   |
| Clean Agile: Back to Basics                    | Robert Martin                | Common   |
| The Clean Coder                                | Robert Martin                | Common   |
| Functional Programming in JavaScript           | Luis Atencio                 | Common   |
| High Performance MySQL                         | Botros, Tinley               | DB       |
| SQL Queries for Mere Mortals                   | Martin Graber                | DB       |
| Introduction to Database Systems               | C.J. Date                    | DB       |
| Базы данных                                    | В.К. Волк                    | DB       |
| Database Processing                            | David M. Kroenke             | DB       |
