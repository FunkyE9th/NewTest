Link to video coming soon.



1.  Update the OS

   ```
   sudo apt update
   sudo apt upgrade
   ```

   

2. Install Dependencies

   ```
   sudo apt install --no-install-recommends git cmake ninja-build gperf \
        ccache dfu-util device-tree-compiler wget \
        python3-dev python3-pip python3-setuptools python3-tk python3-wheel xz-utils file \
        make gcc gcc-multilib g++-multilib libsdl2-dev
   ```

   

3. Get Zephyr and Install Python Dependencies

   - Install west, and make sure ~/.local/bin is on your PATH environment variable

     ```
     pip3 install --user -U west
     echo 'export PATH=~/.local/bin:"$PATH"' >> ~/.bashrc
     source ~/.bashrc
     ```

     

   - Get Zephyr Source Code

     ```
     west init ~/zephyrproject
     cd ~/zephyrproject
     west update
     ```

     

   - Export Zephyr CMake package

     ```
     west zephyr-export
     ```

     

   - Zephyr’s scripts/requirements.txt file declares additional Python dependencies. Install them with pip3

     ```
     pip3 install --user -r ~/zephyrproject/zephyr/scripts/requirements.txt
     ```

     

4. step 4

5. step 5

6. step 6

7. step 7

8. step 8

9. 