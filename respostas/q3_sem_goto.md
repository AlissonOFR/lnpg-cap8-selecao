Atividade 03:
Java:
public class Main {
    public static void main(String[] args) {
        int j = -3;

        for (int i = 0; i < 3 && j <= 0; i++) {

            if (j + 2 == 3 || j + 2 == 2) {
                j--;
            } else if (j + 2 == 0) {
                j += 2;
            } else {
                j = 0;
            }

            if (j <= 0) {
                j = 3 - i;
            }
        }

        System.out.println("j final: " + j);
    }
}

Python:
j = -3
i = 0

while i < 3 and j <= 0:

    if j + 2 == 3 or j + 2 == 2:
        j -= 1
    elif j + 2 == 0:
        j += 2
    else:
        j = 0

    if j <= 0:
        j = 3 - i

    i += 1

print("j final:", j)

Swift:
import Foundation

var j = -3
var i = 0

while i < 3 && j <= 0 {

    if j + 2 == 3 || j + 2 == 2 {
        j -= 1
    } else if j + 2 == 0 {
        j += 2
    } else {
        j = 0
    }

    if j <= 0 {
        j = 3 - i
    }

    i += 1
}

print("j final: \(j)")
