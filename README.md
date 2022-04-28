# Select-the-operation
Propuesta didactica
'''
Ingresar dos números enteros por teclado.
Validar que los números no sean vacíos ni sean caracteres.
Elaborar un programa que contenga un menú con las siguientes opciones:
1 - Sumar los números
2 - Restar los números
3 - Multiplicar los números
4 - Dividir los números
5 - Módulo de División de los números
6 - Salir del programa
De acuerdo a la opción elegida, únicamente mostrar el resultado de la misma.
'''

# Var
print("")
num1 = input("Ingrese Número: ")
num2 = input('Ingrese Número: ')

# Opr
print("")
if len(num1) == 0 or len(num2) == 0:
    print("Debe agregar valores numéricos para ambos casos.")
    print("")
else:
    if num1.isdigit() and num2.isdigit():
        num1Fin = float(num1)
        num2Fin = float(num2)
        print("Que desea hacer?\n1 - Sumar los números\n2 - Restar los números\n3 - Multiplicar los números\n4 - Dividir los números\n5 - Módulo de División de los números\n6 - Salir del programa")
        print("")

        op = input("Ingrese Opción: ")
        print("")
        if len(op) == 0:
            print("Su elección no se encuentra dentro de las opciones sugeridas.")
            print("")
        else:
            if op.isdigit():
                opFin = float(op)
                if opFin ==1:
                    print(num1Fin + num2Fin)
                    print("")
                    print("Gracias por participar.")
                    print("")
                else:
                    if opFin == 2:
                        print(num1Fin - num2Fin)
                        print("")
                        print("Gracias por participar.")
                        print("")
                    else:
                        if opFin == 3:
                            print(num1Fin * num2Fin)
                            print("")
                            print("Gracias por participar.")
                            print("")
                        else:
                            if opFin == 4:
                                if num2Fin == 0:
                                    print("El divisor es igual a 0. Su división no es posible en los números reales.")
                                    print("")
                                    print("Gracias por participar.")
                                    print("")
                                else:
                                    print(num1Fin/num2Fin)
                                    print("")
                                    print("Gracias por participar.")
                                    print("")
                            else:
                                if opFin == 5:
                                    if num2Fin == 0:
                                        print("El divisor es igual a 0. Su división no es posible en los números reales.")
                                        print("")
                                        print("Gracias por participar.")
                                        print("")
                                    else:
                                        print(num1Fin%num2Fin)
                                        print("")
                                        print("Gracias por participar.")
                                        print("")
                                else:
                                    if opFin == 6:
                                        print("Gracias por participar.")
                                        print("")
                                    else:
                                        print("Su elección no se encuentra dentro de las opciones sugeridas.")
                                        print("")
            else:
                print("Su elección no se encuentra dentro de las opciones sugeridas.")
                print("")                            
    else:
        print("Debe agregar valores numéricos para ambos casos.")
        print("")          

# Fin
