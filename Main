#include <iostream>

using namespace std;

template <typename in>
void In(in ** &arr, int lines, int column) {
	for (int i = 0; i < lines; i++) {
		for (int j = 0; j < column; j++) {
			cin >> arr[i][j];
		}
	}
}

template <typename out>
void Out(out ** &arr, int lines, int column) {
	for (int i = 0; i < lines; i++) {
		for (int j = 0; j < column; j++) {
			cout << arr[i][j] << " ";
		}
		cout << endl;
	}
}

template <typename sort>
void Sort(sort ** &arr, int lines, int column, sort element) {
	int iter = 0;
	sort cup;
	while (iter < column) {
		for (int i = 0; i < lines; i++) {
			for (int j = 0; j < column - 1; j++) {
				if (arr[i][j] != element) {

					cup = arr[i][j];
					arr[i][j] = arr[i][j + 1];
					arr[i][j + 1] = cup;

				}
			}
		}
		iter++;
	}
}

int main() {

	int l, c;
	cout << "Enter number of lines ";
	cin >> l;
	cout << endl;
	cout << endl;
	cout << "Enter number of column ";
	cin >> c;
	cout << endl;

	int type;
	int check = 0;

	cout << "What type of matrix you want to chose? " << endl;
	cout << "1) Int matrix" << endl << "2) Float matrix" << endl << "3) Char matrix" << endl;

	while (check == 0) {
		cin >> type;
		cout << endl;
		switch (type) {
		case 1: {

			check++;

			int **matrix1 = new int*[c];
			for (int i = 0; i < c; i++) {
				matrix1[i] = new int[l];
			}

			cout << "Enter elements of matrix: " << endl;
			In(matrix1, l, c);
			cout << endl;

			int element;

			cout << "Which element want you to sort matrix?" << endl;
			cin >> element;
			cout << endl;

			Sort(matrix1, l, c, element);

			cout << "Output matrix: " << endl;
			Out(matrix1, l, c);

			break;
		}
		case 2: {

			check++;

			float **matrix1 = new float*[c];
			for (int i = 0; i < c; i++) {
				matrix1[i] = new float[l];
			}

			cout << "Enter elements of matrix: " << endl;
			In(matrix1, l, c);
			cout << endl;

			float element;

			cout << "Which element want you to sort matrix?" << endl;
			cin >> element;
			cout << endl;

			Sort(matrix1, l, c, element);

			cout << "Output matrix: " << endl;
			Out(matrix1, l, c);

			break;
		}
		case 3: {

			check++;

			char **matrix1 = new char*[c];
			for (int i = 0; i < c; i++) {
				matrix1[i] = new char[l];
			}

			cout << "Enter elements of matrix: " << endl;
			In(matrix1, l, c);
			cout << endl;

			char element;

			cout << "Which element want you to sort matrix?" << endl;
			cin >> element;
			cout << endl;

			Sort(matrix1, l, c, element);

			cout << "Output matrix: " << endl;
			Out(matrix1, l, c);

			break;
		}
		default: {
			cout << "Wrong enter, please try again (number must be in type of integer)" << endl;
		}
		}
	}

	system("pause");
}
