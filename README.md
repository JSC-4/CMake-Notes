# CMake-Notes


## Commands  
This command will generate a buildsystem in the ./build directory (or create it if it's missing) from the source in the ./project directory.  
cmake [&lt;options&gt;] -S &lt;path-to-source&gt; -B &lt;path-to-build&gt;    

Prepopulate cached information  
cmake -C &lt;initial_cache_script&gt; &lt;path-to-source&gt;  

Build project  
cmake --build &lt;dir&gt; -- &lt;build-tool-options&gt;  

Clean project  
cmake --build &lt;dir&gt; -t clean  

Alternative clean project  
cmake --build &lt;dir&gt; --clean-first 

Print text to the standard output. Adding a MODE argument the output can be customised.
message()

Partition CMake code into separate files to keep things ordered and separate.
include()

Include a file only once.
include_guard()

File command will let you read, write, and transfer files and work with the filesystem, file locks, paths, and archives.
file()

Execute_process allows you to run other processes and collect their output, which is usesful in scripts, and it can also be used in projects during the configuration stage.
execute_process()

Create an executable file
add_executable()
