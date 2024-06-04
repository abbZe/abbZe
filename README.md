[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)]
[![TypeScript](https://badges.frapsoft.com/typescript/love/typescript.png?v=101)]

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

const opts: IFullstackDevOpts = {
    name: 'Dmitrii',
    role: 'Fullstack Dev',
    languages: ['ru_RU', 'en_US'],
};

const fullStackDevDima = new FullstackDev(opts);

console.log(fullStackDevDima.greetings());

```
