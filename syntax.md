main: () -> ();


expose fibonacci: usize -> u128;
fibonacci number -> 
let 
    u128 a = 0;
    u128 b = 1;
    u128 c = 1;
in {
    let usize i = 0; in 
    for i < number; i++; {
        a = b;
        b = c;
        c = a + b;
    }
}

