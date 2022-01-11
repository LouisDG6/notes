## Twice as Old
def twice_as_old(dad_years_old, son_years_old):
    print (abs(dad_years_old - 2 * son_years_old))

twice_as_old(36, 7)

## Fake Binary
function fakeBin(x) {
    return x.split('').map(n => n < 5 ? 0 : 1).join('');
}

## Fake Binary (solution 2)
function fakeBin(x) {
  return x.replace(/\d/g, d => d < 5 ? 0 : 1);
}