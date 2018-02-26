#Ask user for names of files to be inputted
fname1 = input("Enter name of file 1:")
fname2 = input("Enter name of file 2:")

 # Open two text files
f1 = open(fname1)
f2 = open(fname2)

#print confirmation for opening files
print("--------------------------------")
print("Comparing files", ">" + fname1, "<" + fname2, sep="\n")
print("--------------------------------")

#read the first line from each file

f1_line = f1.readline()
f2_line = f2.readline()
#initialize the counter for lines
line_no = 1
# loop through the line until EOF
while f1_line != "" or f2_line!="":
    #strip the leading spaces
    f1_line = f1_line.strip()
    f2_line = f2_line.strip()

    if f1_line !=f2_line:

        if f2_line == "" and f1_line !="":
            print(">+", "Line-%s" %line_no,f1_line)
        elif f1_line != "":
            print( ">", "Line-%s" %line_no,f1_line)
        if f1_line == "" and f2_line !="":
            print("<+","Line-%s" %line_no,f2_line)
        elif f2_line != "":
            print("<", "Line-%s" %line_no,f2_line)
        print()
    f1_line = f1.readline()
    f2_line = f2.readline()
    line_no += 1
f1.close()
f2.close()
