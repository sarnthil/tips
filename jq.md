# jq tips

## . (dot, your best friend, yourself)

## get a slice of an array (like in python)

    jq <arrays.json '.[2:7]'

## get an array as a stream

    jq <arrays.json '.[].property'
    jq <arrays.json '.[] | .property'

## turn the stream back into an array

    jq <arrays.json '[.[]]'

never useful, just to show you can do that,
however, this is useful:

    jq <asdas.json '[...]'

where ... is an expression that results into a stream, 
and then through [ ] into an array

## '.property?', '[]?',  '.[].property?'

    jq <foo.json '.property?'
    
when the property doesn't exist, jq doesn't cry

## {} to construct an object

    jq <foo.json '{number: .foo, comment: .bar}'

## .. recursive descent

    jq <array.json '..'

weird, produces all values. 

## read the manual, helps

https://stedolan.github.io/jq/manual/
