# calculadora.py
Projeto básico de calculadora de medicamentos utilizando Python

def calcular_dose(peso, dose_por_kg):
    return peso* dose_por_kg

print("== CALCULADORA DE MEDICAMENTO ==")
try:
    peso = float(input("Informe o peso do paciente (kg)"))
    dose_padrao = float(input("Informe a dose padrão (mg/kg)"))

    dose_total = calcular_dose(peso, dose_padrao)
    print(f"Dose recomendada: {dose_total:.2f} mg")
    print("Obrigada por usar a calculadora de medicamentos!")

except ValueError:
    print("Entrada inválida. Por favor, insira números válidos.")

