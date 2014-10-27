# Qlang

[![Gem Version](https://badge.fury.io/rb/qlang.svg)](http://badge.fury.io/rb/qlang) [![Build Status](https://travis-ci.org/gogotanaka/Q.svg?branch=master)](https://travis-ci.org/gogotanaka/Q) [![Coverage Status](https://coveralls.io/repos/gogotanaka/Q/badge.png?branch=master)](https://coveralls.io/r/gogotanaka/Q?branch=master) [![Code Climate](https://codeclimate.com/github/gogotanaka/Q/badges/gpa.svg)](https://codeclimate.com/github/gogotanaka/Q) [![Dependency Status](https://gemnasium.com/gogotanaka/Q.svg)](https://gemnasium.com/gogotanaka/Q)

## Do you know one of the best language in this world?

#### I belive mathematics is that one absolutely.

## How can we deal such a great mathematics in discret world?

#### Q-language can be.

Q let you know the sense of mathematics with Keyboard same as with a pen.

```
+---Discret world---+                    +------mathematics-----+
|        Ruby       |                    |        axiom         |
|        TeX        |<------   Q  ------>|    Uncountable noun  |
|       Pyhthon     |                    |  real number topology|
+-------------------+                    +----------------------+
```

## Demo

Below code is input and output for interpreter of q-lang

(you can try it by `qlang -i`)

### Differentiate

```
d/dx(cos(x))
=> ( - sin( x ) )

d/dx(log(x))
=> ( 1 / x )

# You can omit parentheses

d/dy y^2                        
=> ( 2 * y )

d/dy xy                       
=> ( x )
```


### Integrate

```
S(log(x)dx)[0..1]
=> - oo

S(sin(x)dx)[0..pi]
=> 2.0

S(cos(x)dx)[0..pi]                       
=> 0.0
```


### Matrix

```
(1 2 3; 4 5 6)
=> (1 2 3; 4 5 6)

(1 2 3; 4 5 6) + (1 2 3; 4 5 6)
=> (2 4 6; 8 10 12)

(1 2 3; 4 5 6) * (1 2 3)
=> (14 32)
```

### Function
```
f(x, y) = xy
f(1, 2)
=> 2
```


## How to use

Install qlang gme.

    $ gem install qlang
    
    
## Use as native language

### Compile into R

    $ qlang -r foo.q
    
### Compile into Ruby

    $ qlang -rb foo.q
    
### Compile into Python

    $ qlang -py foo.q


## Use as math template within other langs


```rb
class ExampleClass
  def example_method
    #your Ruby codes
    ......

I love mathematics.
  a = (1 3 4)
  # your Q codes
Q.E.D

  end
end
```

    $ qlang -rb example.rb
    

```rb
class ExampleClass
  def example_method
    #your Ruby codes
    ......

    a = Vector[1, 3, 4]

  end
end
```

## Interpreter

    $ qlang -i
    Q:-> 

## Contributing

Welcome any your PR or issue.
You can become commiter, if you commit even once.
