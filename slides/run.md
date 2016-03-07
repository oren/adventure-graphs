## Initialize Cayley
```
cayley init -db=bolt -dbpath=./testdb
```

## Run the REPL
```
cayley repl -db=bolt -dbpath=./testdb
```

## Run the web frontend
```
cayley http -db=bolt -dbpath=./testdb
```

## Use a configuration file

Create this config file: cayley.cfg
```
{
"database": "bolt",
"db_path": "./testdb"
}
```

Now you can run `init`, `repl`, and `http` using the --config argument:
```
cayley init --config=cayley.cfg
cayley repl --config=cayley.cfg
cayley http --config=cayley.cfg
```
