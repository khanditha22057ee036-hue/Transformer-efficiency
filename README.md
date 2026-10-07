# Transformer Efficiency Calculation
# Formula: Efficiency = (Output Power / Input Power) * 100

output_power = float(input("Enter output power (W): "))
losses = float(input("Enter total losses (W): "))

if output_power < 0 or losses < 0:
    print("Power and losses cannot be negative.")
else:
    input_power = output_power + losses
    efficiency = (output_power / input_power) * 100

    print("Input Power =", round(input_power, 2), "W")
    print("Transformer Efficiency =", round(efficiency, 2), "%")