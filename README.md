# caim

caim is a terminal base [Zaim](https://zaim.net/) client.

## Installation

### Dependencies

- ruby
- bundler

### Install

Clone this repository and

    $ bundle install --path vendor/bundle
    $ bundle exec ./bin/caim login

## Usage

Get list

    $ caim list
    $ caim list 2017-11

    2017-11-01 458 食費 昼ごはん
    2017-11-01 195 交通費 バス
    ...


Pay payment

    $ caim pay 150 --genre genre_id --account 財布 --date 2017-11-23 --comment コカコーラ --place セブンイレブン一番町店
    $ caim pay 150 -g genre_id


## TODO


cache categories, genres and accounts

    $ caim category update
    $ caim category show

    id name ...

income

    $ caim earn 200000 給与収入

filter

    $ caim list --category 食費

summary

    $ caim sum 2017-11
    $ caim sum 2017-11 -c 食費

    2000

total amounts of each account

    $ caim account

    財布 2000
    口座 20
    クレジット -10000
    ...



## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
