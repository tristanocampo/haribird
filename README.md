# haribird

To compile and run the F-Bird game on DOSBox, follow these steps:

**1.) Download and Install NASM (Netwide Assembler)**

**2.) Get the F-Bird Source Code:**

  You can either clone the repository using git clone https://github.com/nanochess/fbird.git or download the file directly.

**3.) Prepare Your Environment:**

Create a directory to store the F-Bird source code and the compiled binary. For example, create a directory named fbird on your local machine.

**4.) Assemble the Source Code:**

Open a command prompt or terminal. Navigate to the directory where fbird.asm is located.
Run the following command to assemble the source code into a COM file:

      nasm -f bin fbird.asm -o fbird.com

**5.)Set Up DOSBox:**

Install DOSBox if you haven't already. Create a directory on your machine to use as a virtual C: drive for DOSBox, for example, C:\DOSBox\CDrive.
Copy the fbird.com file into this directory.

**6.) Run F-Bird in DOSBox:**

Open DOSBox.
Mount the directory you created as the C: drive by entering the following command in DOSBox:

    mount c C:\DOSBox\CDrive
    
Change to the C: drive by entering:

     c:

Navigate to the directory containing fbird.com if it is in a subdirectory.
Run the game by typing:


    fbird.com
