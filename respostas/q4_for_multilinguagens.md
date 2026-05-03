Atividade 04:
Python:
n = 100
i = 0
j = 17
sum = 0

while i < n:
    sum += i * j + 3
    i += 1
    j -= 1

print(sum)

C:
#include <stdio.h>

int main() {
    int i, j, n = 100;
    int sum = 0;

    for (i = 0, j = 17; i < n; i++, j--) {
        sum += i * j + 3;
    }

    printf("%d\n", sum);
    return 0;
}
Haskell:
main :: IO ()
main = print (loop 0 17 100 0)

loop :: Int -> Int -> Int -> Int -> Int
loop i j n sum
    | i >= n    = sum
    | otherwise = loop (i + 1) (j - 1) n (sum + i * j + 3)

Ruby:
n = 100
j = 17
sum = 0

(0...n).each do |i|
  sum += i * j + 3
  j -= 1
end

puts sum

Swift:
import Foundation

var n = 100
var j = 17
var sum = 0

for i in 0..<n {
    sum += i * j + 3
    j -= 1
}

print(sum)
