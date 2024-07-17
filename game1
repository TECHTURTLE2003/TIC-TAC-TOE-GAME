*********This is the basic TIC TAC TOE game .I have to do this game project by using java programming language. 
package project;
import java.util.*;

public class Tic_Tac_Toe {
   //Initialize the matrix
	public static void main(String[] args) {
		char[][] Ticboard = new char[3][3];
		for (int row = 0; row < Ticboard.length; row++) {
			for (int col = 0; col < Ticboard[row].length; col++) {
				Ticboard[row][col] = ' ';
			}
		}
		char p1 = 'X';
		boolean gameOver = false;
		Scanner scanner = new Scanner(System.in);
  //repeatative checking the matrix
		while (gameOver !=false) {
			printBoard(Ticboard);
			System.out.print("Player " + p1 + " enter: ");
			int row = scanner.nextInt();
			int col = scanner.nextInt();
			System.out.println();

			if (Ticboard[row][col] == ' ') {
				Ticboard[row][col] = p1; // place the element
				gameOver = haveWon(Ticboard, p1);
				if (gameOver) {
					System.out.println("Player " + p1 + "has won the game....... ");
				} else {
					 if (p1 == 'X') {
					 p1 = 'O';
					 } else {
					 p1 = 'X';
					 }
				}
			} else {
				System.out.println("Invalid move. Please Try again!!!!!");
			}
		}
	}
   // Check the iteration for every time
	private static boolean haveWon(char[][] board, char player) {
		for (int row = 0; row < board.length; row++) {
			if (board[row][0] == player && board[row][1] == player && board[row][2] == player) {
				return true;
			}
		}
		for (int col = 0; col < board.length; col++) {
			if (board[0][col] == player && board[1][col] == player && board[2][col] == player) {
				return true;

			}
		}
		if (board[0][0] == player && board[1][1] == player && board[2][2] == player) {
			return true;
		}
		if (board[0][2] == player && board[1][1] == player && board[2][0] == player) {
			return true;
		}

		return false;
	}
  // Print the matrix 
	public static void printBoard(char[][] board) {
		for (int row = 0; row < board.length; row++) {
			for (int col = 0; col < board[row].length; col++) {
				System.out.print(board[row][col] + " | ");
			}
			System.out.println();
		}
	}
}
