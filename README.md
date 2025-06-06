import webbrowser

def main():
    # Ask how many Chrome windows to open, with error handling
    while True:
        try:
            num = int(input("How many Chrome windows do you want to open? (e.g., 4): "))
            break
        except ValueError:
            print("Please enter a valid number.")

    for i in range(num):
        webbrowser.open_new("https://www.youtube.com/watch?v=wN-mZtbX2Pg")

if __name__ == "__main__":
    main()
