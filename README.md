# Nim-Game
You are playing the following Nim Game with your friend:

Initially, there is a heap of stones on the table.
You and your friend will alternate taking turns, and you go first.
On each turn, the person whose turn it is will remove 1 to 3 stones from the heap.
The one who removes the last stone is the winner.
Given n, the number of stones in the heap, return true if you can win the game assuming both you and your friend play optimally, otherwise return false.
 
Input
There will be a single line of input n representing the number.

Constraints
1 ≤ n ≤ 231 - 1
Output
Print true if you can win the game assuming both you and your friend play optimally, otherwise print false.

def canWinNim(n):
    return n % 4 != 0

if __name__ == "__main__":
    n = int(input().strip())
    print("true" if canWinNim(n) else "false")
