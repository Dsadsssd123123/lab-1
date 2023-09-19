#include <iostream>
#include <vector>

int main() {
    int N; // Розмір масиву
    std::cout << "Введіть розмір масиву: ";
    std::cin >> N;

    std::vector<int> A(N); 

   
    std::cout << "Введіть елементи масиву A:" << std::endl;
    for (int i = 0; i < N; i++) {
        std::cin >> A[i];
    }

    std::vector<int> positiveElements; 

    for (int i = 0; i < N; i++) {
        if (A[i] >= 0) {
            positiveElements.push_back(A[i]);
        }
    }

    std::cout << "Позитивні елементи масиву A:" << std::endl;
    for (int i = 0; i < positiveElements.size(); i++) {
        std::cout << positiveElements[i] << " ";
    }

    return 0;
}
