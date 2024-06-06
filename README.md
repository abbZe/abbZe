#Intro

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

#My library
| Book | Author | Was read?
| ----------- | Common | ----------- |
| Clean Code | Robert Martin | [x] |
| Clean Architecture | Robert Martin | [x] |
| Code Complete| Steve McConnel | [x] |
| Extreme programming | Kent Beck | [x] | 
| JavaScript Patterns | Stoyan Stefanov | [x] |
| Clean Agile: Back to Basics | Robert Martin | [x] |
| The Clean Coder | Robert Martin | [x] |
| Functional Programming in JavaScript | Luis Atencio | [x] |
| ----------- | DB | ----------- |
| High Performance MySQL | Botros, Tinley | [x] |
| SQL Queries for Mere Mortals | Martin Graber | [x] |
| Introduction to Database Systems | C.J.Date | [x] |
| Базы данных: проектирование, программирование, управление и администрирование | В.К.Волк | [x] |
| Database Processing | David M. Kroenke | [x] |
