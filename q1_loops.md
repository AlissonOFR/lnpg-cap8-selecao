# lnpg-cap8-selecao
Atividade Estrutura de Seleção
Java:
public class Main {
    public static void main(String[] args) {
        int j = 5; 
        int k = (j + 13) / 27;

        while (k <= 10) {
            k = k + 1;
            int i = 3 * k - 1;
            System.out.println("k = " + k + ", i = " + i);
        }

        System.out.println("Fim do loop.");
    }
}

Python:
def main():
    j = 5  # valor de exemplo
    k = (j + 13) // 27

    while k <= 10:
        k = k + 1
        i = 3 * k - 1
        print(f"k = {k}, i = {i}")

    print("Fim do loop.")

if __name__ == "__main__":
    main()

Haskell:
main :: IO ()
main = do
    let j = 5
    let k = (j + 13) `div` 27
    loop k
    putStrLn "Fim do loop."

loop :: Int -> IO ()
loop k =
    if k > 10
        then return ()
        else do
            let k' = k + 1
            let i = 3 * k' - 1
            putStrLn ("k = " ++ show k' ++ ", i = " ++ show i)
            loop k'



Swift:
import Foundation

let j = 5 // valor de exemplo
var k = (j + 13) / 27

while k <= 10 {
    k = k + 1
    let i = 3 * k - 1
    print("k = \(k), i = \(i)")
}

print("Fim do loop.")
