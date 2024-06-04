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
