main: () -> ();

# Functions
expose fibonacci: usize number -> u128;
fibonacci -> 
    let 
        usize a, b = 0;
        usize c = 1;
    in {
    for let i = 0; i < number; i++; {
        a = b;
        b = c;
        c = a + b;
    }
    return a;
}

(
    (100, 200) => add,
    300,
) => add => fibonacci;

# Lambdas
($x + $y) = seq: Int x -> x + 1;
$x,y -> x + y == ($x + $y);
