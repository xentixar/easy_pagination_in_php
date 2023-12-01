# Easy PHP Pagination

This is a simple PHP library for easy pagination in PHP.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository or download the ZIP file.

```bash
git clone https://github.com/xentixar/easy_pagination_in_php.git
```

2. Configure database in database.php inside config directory.

```php
private $database_name = 'your_database_name';
```

3. Include autoload.php file in your file

```bash
require_once __DIR__ . '/autoload.php';
```

## Usage

1. Fetch data from table or from any other source as array.

For example: 

```php
$data = [
    'data_1','data_2','data_3'
];
```

2. Adjust the `$limit` variable in the PHP script to control the number of records displayed per page.

```php
$limit = 10;
```

3. Create an instance of the Class class and pass data and limit to it.

```php
$paginator = new Pagination($data, $limit);
```

4. Get the paginated data using the paginate method.

```php
$paginated_data = $paginator->paginate();
```

5. View the pagination links using the links method.

```php
$paginator->links();
```

## Examples

Check the example directory for sample usage of the pagination library.


## Contributing

* Fork the repository.
* Create a new branch: git checkout -b feature-name.
* Commit your changes: git commit -m 'Add new feature'.
* Push to the branch: git push origin feature-name.
* Submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

