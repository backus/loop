I use [filewatcher](https://github.com/thomasfl/filewatcher) a lot. Usually I do something like this

```sh
$ filewatcher 'spec/unit/foo/bar_spec.rb' 'bundle exec rspec spec/unit/foo/bar_spec.rb'
```

In cases like this I want something even simpler

```sh
$ loop bundle exec rspec spec/unit/foo/bar_spec.rb
```

`loop` just watches the files it finds in the arguments you give it. Pretty simple.
