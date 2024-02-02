

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


