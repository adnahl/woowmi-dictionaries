# woowmi-dictionaries

A multilingual dictionary for the Woowmi project. This repository contains translation files for different languages that can be edited by the community.

## Available Languages

- **English** (`en.json`)
- **Spanish** (`es.json`)

## Structure

Each translation file is a JSON object with key-value pairs where:
- **Key**: A unique identifier for the translation (same across all languages)
- **Value**: The translated text in the respective language

Example:
```json
{
  "welcome": "Welcome",
  "hello": "Hello",
  "goodbye": "Goodbye"
}
```

## Contributing

We welcome contributions from the community! You can help by:

1. **Adding new translations**: Add new key-value pairs to existing language files
2. **Improving existing translations**: Update translations to be more accurate or natural
3. **Adding new languages**: Create a new JSON file for your language (e.g., `fr.json` for French)

### Guidelines

- **Keep keys consistent**: All language files must have the same keys
- **Use snake_case**: Keys should use lowercase letters with underscores (e.g., `thank_you`)
- **Be descriptive**: Keys should clearly indicate their purpose
- **Valid JSON**: Ensure your file is valid JSON format
- **UTF-8 encoding**: Use UTF-8 encoding for special characters

### How to Contribute

1. Fork this repository
2. Edit the translation file(s)
3. Ensure all language files have the same keys
4. Validate your JSON syntax
5. Submit a pull request with a clear description of your changes

## Usage

To use these translations in your project:

```javascript
// Example in JavaScript
import en from './en.json';
import es from './es.json';

const translations = { en, es };
const currentLang = 'en';
const t = (key) => translations[currentLang][key];

console.log(t('welcome')); // Output: "Welcome"
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.