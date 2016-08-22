## Original requirements

Реализовать банкомат для выдачи монет.
1) При инициализации он должен принимать количество монет каждого номинала в наличии (например, 10 монет по "50", 8 монет по "25" и т.д.). Номиналы бывают: 1, 2, 5, 10, 25, 50.

2) Реализовать метод который принимает сумму для выдачи и возвращает определённое количество монет нужного номинала. Если в наличии нет подходящего количества нужных монет - пользователь должен получить сообщение об этом.

Например, если поступил запрос на выдачу 2 грн, а в наличии есть 3 монеты по "50" и 4 монеты по "25", то результат может быть таким: {50 => 3, 25 => 2} или {50 => 2, 25 => 4}.
Если я прошу выдать 20 копеек - должен вернуть сообщение об ошибке.

Количество монет в наличии должно уменьшаться после каждого размена. Также нужна возможность пополнять монеты в наличии

3) Задачу оформить в виде RESTful API.

## HOWTO

`$ bundle install`

`$ bundle exec rspec`

`$ bundle exec rackup`

`$ bundle exec mutant --use rspec MoneyChecker Atm`