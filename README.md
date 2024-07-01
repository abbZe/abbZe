![Welcome to my profile!](https://github.com/abbZe/profile-images/blob/main/welcome.png?raw=true)

![TypeScript](https://badges.frapsoft.com/typescript/love/typescript.svg?v=101)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)
![Fedora linux](https://img.shields.io/badge/Fedora-294172?style=for-the-badge&logo=fedora&logoColor=white)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=abbZe.abbZe)

## Мое оригинальное приветствие, демонстрирующее принципы SOLID :)
```typescript
/**
 * (S) единая ответственность
 * (I) специфичность интерфейса
 */ 
interface IDev {
    greetings: () => string;
}

interface IDevOpts {
    name: string;
    role: string;
    languages: Languages[];
}

enum Languages {
    RU = 'ru_RU',
    EN = 'en_US'
}

/**
 * (O) Открыт для расширения, закрыт для модификации
 * (L) Не демонстрирую напрямую, так как нужен наследник, но FullStackDev можно заменить любым классом, наследующимся от IDev
 * (D) Опции не захардкожены, а инжектированы (обычно демонстрация идет на классах, но тут опции пусть будут)
 */ 
class FullStackDev implements IDev {
    public readonly name: string;
    public readonly role: string;
    public readonly languages: Languages[];

    constructor({ name, role, languages }: IDevOpts) {
        this.name = name;
        this.role = role;
        this.languages = languages;
    }

    public greetings() {
        return `Благодарю за посещение профиля ${this.name}, надеюсь вы нашли что-то интересное для себя :)`;
    }
}


const dimaOpts: IDevOpts = {
    name: 'Дмитрий',
    role: 'Fullstack Dev',
    languages: [Languages.RU, Languages.EN], // Использование перечисления для языков
};

const fullStackDevDima: IDev = new FullStackDev(dimaOpts);
console.log(fullStackDevDima.greetings())
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
