# SecuriSearch

SecuriSearch is a web application built with Symfony that provides a searchable glossary of cybersecurity terms. Users can enter a term in the search bar and receive a simple, understandable explanation of cybersecurity terminology.

## Features

- **Searchable Glossary**: Users can search for cybersecurity terms and view definitions.
- **Expandable**: Easily add new terms or categories as the glossary grows.
- **User-Friendly Interface**: Simple, intuitive interface for quick searches.

## Getting Started

### Prerequisites

- PHP 8.x
- Composer
- Symfony CLI
- MySQL (or another compatible database)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/securisearch.git
    cd securisearch
    ```

2. Install dependencies:
    ```bash
    composer install
    ```

3. Set up the database:
   - Configure the database URL in the `.env` file:
     ```
     DATABASE_URL="mysql://user:password@127.0.0.1:3306/securisearch"
     ```
   - Create the database and run migrations:
     ```bash
     php bin/console doctrine:database:create
     php bin/console doctrine:migrations:migrate
     ```

4. Load sample data (optional):
    ```bash
    php bin/console doctrine:fixtures:load
    ```

5. Run the Symfony server:
    ```bash
    symfony serve
    ```

6. Visit the application at `http://127.0.0.1:8000/search`.

### Usage

1. Open the search page.
2. Enter a cybersecurity term (e.g., "SOC" or "SIEM").
3. View the term's definition.

## License

This project is licensed under the MIT License.

---

Happy learning with SecuriSearch!
