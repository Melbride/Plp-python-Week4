def read_and_write_file():
    try:
        # Ask the user for the input file name
        input_filename = input("Enter the name of the file to read: ")

        # Try to open and read the file
        with open(input_filename, 'r') as infile:
            content = infile.read()

        # make the content uppercase
        modified_content = content.upper()

        # Create a new output file name
        output_filename = "modified_" + input_filename

        # Write the modified content to the new file
        with open(output_filename, 'w') as outfile:
            outfile.write(modified_content)

        print(f"\n✅ File successfully read and modified content saved to '{output_filename}'.")

    except FileNotFoundError:
        print("❌ Error: The file does not exist. Please check the filename and try again.")
    except IOError:
        print("❌ Error: An I/O error occurred while reading or writing the file.")
    except Exception as e:
        print(f"❌ An unexpected error occurred: {e}")

# Run the function
read_and_write_file()
