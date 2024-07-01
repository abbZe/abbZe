![Welcome to my profile!](https://github.com/abbZe/profile-images/blob/main/welcome.png?raw=true)

![TypeScript](https://badges.frapsoft.com/typescript/love/typescript.svg?v=101)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)
![Fedora linux](https://img.shields.io/badge/Fedora-294172?style=for-the-badge&logo=fedora&logoColor=white)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=abbZe.abbZe)

# Мое оригинальное приветствие, демонстрирующее принципы SOLID :)
```typescript
enum Languages {
    RU = 'ru_RU',
    EN = 'en_US',
}

enum Roles {
    FULLSTACK = 'FullStack',
    FRONTEND = 'Frontend',
    BACKEND = 'Backend',
}

interface IDev {
    greetings(): string;
    doJob(): void;
}

interface IDevOpts {
    name: string;
    role: Roles;
    languages: Languages[];
}

abstract class Dev implements IDev {
    public readonly name: string;
    public readonly role: Roles;
    public readonly languages: Languages[];

    constructor({ name, role, languages }: IDevOpts) {
        this.name = name;
        this.role = role;
        this.languages = languages;
    }

    public greetings(): string {
        return `Благодарю за посещение профиля ${this.name}, надеюсь вы нашли что-то интересное для себя :)`;
    }

    abstract doJob(): void;
}

class FullStackDev extends Dev {
    constructor(opts: IDevOpts) {
        super(opts);
    }

    public doJob = () => {
        console.log(`Работаю над фронтендом и бэкэндом, моё имя ${this.name}`);
    };
}

class FrontendDev extends Dev {
    constructor(opts: IDevOpts) {
        super(opts);
    }

    public doJob = () => {
        console.log(`Работаю над фронтендом, моё имя ${this.name}`);
    };
}

const dimaOpts = {
    name: 'Дмитрий',
    role: Roles.FULLSTACK,
    languages: [Languages.RU, Languages.EN],
};

const annaOpts = {
    name: 'Анна',
    role: Roles.FRONTEND,
    languages: [Languages.RU],
};

const dima = new FullStackDev(dimaOpts);
const anna = new FrontendDev(annaOpts);

console.log(dima.greetings());
console.log(anna.greetings());

console.log(dima.doJob());
console.log(anna.doJob());

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
