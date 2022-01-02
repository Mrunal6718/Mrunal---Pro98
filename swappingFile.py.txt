def swapFileData():

    file1 = input("Enter 1st file name - ")
    file2 = input("Enter 2nd file name - ")

    File1 = open(file1, 'r')
    fileOneText = File1.read()

    File2 = open(file2, 'r')
    fileTwoText = File2.read()
    
    print("Data Of The Files Has Been Swapped")

    write1 = open(file1, 'w')
    write1.write(fileTwoText)

    write2 = open(file2, 'w')
    write2.write(fileOneText)

swapFileData()