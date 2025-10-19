# task-6.2-A-text-file-log.txt-containing-logs-of-a-system.-
Write a function that counts the number of lines containing the word "ERROR".
def count_error_lines(filename):
    error_count = 0
    with open(filename, "r") as file:
        for line in file:
            if "ERROR" in line:
                error_count += 1
    return error_count
error_lines = count_error_lines("log.txt")
print(f"Number of lines with 'ERROR': {error_lines}")
