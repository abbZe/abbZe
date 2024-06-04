```
interface IFullstackDev {
    name: string;
    role: string;
    languages: string[];
}

interface IOpts {
    name: string;
    role: string;
    languages: string[];
}

class FullstackDev implements IFullstackDev {
    name: string;
    role: string;
    languages: string[];

    constructor({ name, role, languages }: IOpts) {
        this.name = name;
        this.role = role;
        this.languages = languages;
    }

    greetings() {
        return `Благодарю за посещение моего профиля,
                надеюсь вы нашли что-то интересное для себя :)`;
    }
}

const opts: IOpts = {
    name: 'Dmitrii',
    role: 'Fullstack Dev',
    languages: ['ru_RU', 'en_US'],
};

const fullStackDevDima = new FullstackDev(opts);

fullStackDevDima.greetings();
```
