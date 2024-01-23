#include <iostream>

// Variables globales
float valor1 = 0;
float valor2 = 0;
float resultado = 0;

// Declaración de funciones
float suma(float a, float b);
float resta(float a, float b);
float multiplicacion(float a, float b);
float division(float a, float b);

int main() {
    // Solicitar al usuario que ingrese dos valores
    std::cout << "Ingrese el primer numero: ";
    std::cin >> valor1;

    std::cout << "Ingrese el segundo numero: ";
    std::cin >> valor2;

    // Llamadas a funciones y asignación de resultados
    resultado = suma(valor1, valor2);
    std::cout << "Suma: " << resultado << std::endl;

    resultado = resta(valor1, valor2);
    std::cout << "Resta: " << resultado << std::endl;

    resultado = multiplicacion(valor1, valor2);
    std::cout << "Multiplicacion: " << resultado << std::endl;

    // Verificar la división por cero antes de realizar la operación
    if (valor2 != 0) {
        resultado = division(valor1, valor2);
        std::cout << "Division: " << resultado << std::endl;
    } else {
        std::cout << "Error: Division por cero." << std::endl;
    }

    return 0;
}

// Definición de funciones
float suma(float a, float b) {
    return a + b;
}

float resta(float a, float b) {
    return a - b;
}

float multiplicacion(float a, float b) {
    return a * b;
}

float division(float a, float b) {
    return a / b;
}
