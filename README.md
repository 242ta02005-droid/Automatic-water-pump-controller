# Automatic-water-pump-controller
# Automatic Water Pump Controller

print("AUTOMATIC WATER PUMP CONTROLLER")
print("--------------------------------")

while True:
    level = float(input("\nEnter water level (%): "))

    if level < 30:
        print("Water level is LOW")
        print("Pump: ON")
        
    elif level >= 90:
        print("Water tank is FULL")
        print("Pump: OFF")
        
    else:
        print("Water level is NORMAL")
        print("Pump: OFF")

    choice = input("\nDo you want to check again? (yes/no): ")

    if choice.lower() != "yes":
        print("Controller stopped.")
        break
