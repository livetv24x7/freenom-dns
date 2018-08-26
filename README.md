## Installation

Add this line to your application's Gemfile:

```ruby
gem 'freenom-dns'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install freenom-dns

## Usage

### Initialize the DNS object

```ruby
dns = Freenom::DNS.new(
  username: freenom_username,
  password: freenom_password,
  domain: freenom_domain
)
```

### List all DNS records

```ruby
dns.records
```

### Create a DNS record

```ruby
dns.create_record!(
  name: record_name,
  type: record_type,
  time_to_live: record_time_to_live,
  target: record_target
)
```

### Delete a DNS record

```ruby
dns.delete_record!(
  (optional) name: record_name,
  (optional) type: record_type,
  (optional) time_to_live: record_time_to_live,
  (optional) target: record_target
)
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/thongncvn/freenom-dns.
