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
