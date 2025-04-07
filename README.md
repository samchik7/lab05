<фрагмент_вставки_значка>
# lab03
export GITHUB_USERNAME=samchik7



cd ${GITHUB_USERNAME}/workspace
~/samchik7/workspace ~/samchik7/workspace
source scripts/activate




git clone https://github.com/${GITHUB_USERNAME}/lab02.git projects/lab03
Cloning into 'projects/lab03'...
remote: Enumerating objects: 19, done.
remote: Counting objects: 100% (19/19), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 19 (delta 2), reused 8 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (19/19), 5.38 KiB | 5.38 MiB/s, done.
Resolving deltas: 100% (2/2), done.
git remote remove origin
git remote add origin https://github.com/${GITHUB_USERNAME}/lab03.git



g++ -std=c++11 -I./include -c sources/print.cpp
ls print.o
print.o
nm print.o | grep print
0000000000000000 T __Z5printRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEERNS_13basic_ostreamIcS2_EE
0000000000000078 T __Z5printRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEERNS_14basic_ofstreamIcS2_EE
ar rvs print.a print.o
ar: creating archive print.a
a - print.o
file print.a
print.a: current ar archive random library
g++ -std=c++11 -I./include -c examples/example1.cpp
ls example1.o
example1.o
g++ example1.o print.a -o example1
./example1 && echo
hello




g++ -std=c++11 -I./include -c examples/example2.cpp
nm example2.o
0000000000000684 s GCC_except_table0
000000000000069c s GCC_except_table1
00000000000006bc s GCC_except_table15
                 U __Unwind_Resume
                 U __Z5printRKNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEERNS_14basic_ofstreamIcS2_EE
0000000000000490 T __ZNSt3__111char_traitsIcE3eofB8ne180100Ev
0000000000000560 T __ZNSt3__111char_traitsIcE6lengthB8ne180100EPKc
                 U __ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6__initEPKcm
0000000000000260 T __ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEC1B8ne180100ILi0EEEPKc
00000000000004cc T __ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEC2B8ne180100ILi0EEEPKc
                 U __ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev
                 U __ZNSt3__113basic_filebufIcNS_11char_traitsIcEEE4openEPKcj
                 U __ZNSt3__113basic_filebufIcNS_11char_traitsIcEEEC1Ev
                 U __ZNSt3__113basic_filebufIcNS_11char_traitsIcEEED1Ev
000000000000039c T __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEEC2B8ne180100EPNS_15basic_streambufIcS2_EE
                 U __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED2Ev
00000000000000fc T __ZNSt3__114basic_ofstreamIcNS_11char_traitsIcEEEC1EPKcj
0000000000000294 T __ZNSt3__114basic_ofstreamIcNS_11char_traitsIcEEED1Ev
00000000000002d4 T __ZNSt3__114basic_ofstreamIcNS_11char_traitsIcEEED2Ev
000000000000063c T __ZNSt3__116__non_trivial_ifILb1ENS_9allocatorIcEEEC2B8ne180100Ev
0000000000000524 T __ZNSt3__117__compressed_pairINS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE5__repES5_EC1B8ne180100INS_18__default_init_tagESA_EEOT_OT0_
0000000000000594 T __ZNSt3__117__compressed_pairINS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE5__repES5_EC2B8ne180100INS_18__default_init_tagESA_EEOT_OT0_
0000000000000650 T __ZNSt3__118__constexpr_strlenB8ne180100EPKc
00000000000005d0 T __ZNSt3__122__compressed_pair_elemINS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE5__repELi0ELb0EEC2B8ne180100ENS_18__default_init_tagE
00000000000005e4 T __ZNSt3__122__compressed_pair_elemINS_9allocatorIcEELi1ELb1EEC2B8ne180100ENS_18__default_init_tagE
                 U __ZNSt3__18ios_base4initEPv
                 U __ZNSt3__18ios_base5clearEj
0000000000000498 T __ZNSt3__18ios_base8setstateB8ne180100Ej
0000000000000428 T __ZNSt3__18ios_baseC2B8ne180100Ev
0000000000000610 T __ZNSt3__19allocatorIcEC2B8ne180100Ev
000000000000044c T __ZNSt3__19basic_iosIcNS_11char_traitsIcEEE4initB8ne180100EPNS_15basic_streambufIcS2_EE
00000000000003fc T __ZNSt3__19basic_iosIcNS_11char_traitsIcEEE8setstateB8ne180100Ej
0000000000000360 T __ZNSt3__19basic_iosIcNS_11char_traitsIcEEEC2B8ne180100Ev
                 U __ZNSt3__19basic_iosIcNS_11char_traitsIcEEED2Ev
                 U __ZSt9terminatev
                 U __ZTTNSt3__114basic_ofstreamIcNS_11char_traitsIcEEEE
                 U __ZTVNSt3__114basic_ofstreamIcNS_11char_traitsIcEEEE
                 U __ZTVNSt3__18ios_baseE
                 U __ZTVNSt3__19basic_iosIcNS_11char_traitsIcEEEE
0000000000000338 T __ZTv0_n24_NSt3__114basic_ofstreamIcNS_11char_traitsIcEEED1Ev
0000000000000674 T ___clang_call_terminate
                 U ___cxa_begin_catch
                 U ___gxx_personality_v0
                 U ___stack_chk_fail
                 U ___stack_chk_guard
0000000000000000 T _main
                 U _strlen
00000000000006cc s l_.str
00000000000006d4 s l_.str.1
0000000000000000 t ltmp0
0000000000000684 s ltmp1
00000000000006cc s ltmp2
00000000000006e0 s ltmp3
g++ example2.o print.a -o example2 
./example2
cat log.txt && echo
hello




rm -rf example1.o example2.o print.o
rm -rf print.a
rm -rf example1 example2
rm -rf log.txt




cat > CMakeLists.txt <<EOF
cmake_minimum_required(VERSION 3.4)
project(print)
EOF




cat >> CMakeLists.txt <<EOF
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
EOF




cat >> CMakeLists.txt <<EOF
add_library(print STATIC \${CMAKE_CURRENT_SOURCE_DIR}/sources/print.cpp)
EOF




cat >> CMakeLists.txt <<EOF
include_directories(\${CMAKE_CURRENT_SOURCE_DIR}/include)
EOF




cmake -H. -B_build
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.


-- The C compiler identification is AppleClang 16.0.0.16000026
-- The CXX compiler identification is AppleClang 16.0.0.16000026
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done (1.4s)
-- Generating done (0.0s)
-- Build files have been written to: /Users/sam/samchik7/workspace/projects/lab03/_build
cmake --build _build
[ 50%] Building CXX object CMakeFiles/print.dir/sources/print.cpp.o
[100%] Linking CXX static library libprint.a
[100%] Built target print





cmake --build _build
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.


-- Configuring done (0.0s)
-- Generating done (0.0s)
-- Build files have been written to: /Users/sam/samchik7/workspace/projects/lab03/_build
[ 33%] Built target print
[ 50%] Building CXX object CMakeFiles/example1.dir/examples/example1.cpp.o
[ 66%] Linking CXX executable example1
[ 66%] Built target example1
[ 83%] Building CXX object CMakeFiles/example2.dir/examples/example2.cpp.o
[100%] Linking CXX executable example2
[100%] Built target example2
cmake --build _build --target print
[100%] Built target print
cmake --build _build --target example1
[ 50%] Built target print
[100%] Built target example1
cmake --build _build --target example2
[ 50%] Built target print
[100%] Built target example2





ls -la _build/libprint.a
-rw-r--r--  1 sam  staff  15352 10 мар 19:31 _build/libprint.a
 _build/example1 && echo
hello
_build/example2
cat log.txt && echo
hello
rm -rf log.txt





git clone https://github.com/tp-labs/lab03 tmp 
Cloning into 'tmp'...
remote: Enumerating objects: 91, done.
remote: Counting objects: 100% (30/30), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 91 (delta 23), reused 21 (delta 21), pack-reused 61 (from 1)
Receiving objects: 100% (91/91), 1.02 MiB | 1.94 MiB/s, done.
Resolving deltas: 100% (41/41), done.
mv -f tmp/CMakeLists.txt .
rm -rf tmp




cat CMakeLists.txt
cmake_minimum_required(VERSION 3.4)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
option(BUILD_EXAMPLES "Build examples" OFF)
project(print)
add_library(print STATIC ${CMAKE_CURRENT_SOURCE_DIR}/sources/print.cpp)
target_include_directories(print PUBLIC
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
  $<INSTALL_INTERFACE:include>
)
if(BUILD_EXAMPLES)
  file(GLOB EXAMPLE_SOURCES "${CMAKE_CURRENT_SOURCE_DIR}/examples/*.cpp")
  foreach(EXAMPLE_SOURCE ${EXAMPLE_SOURCES})
    get_filename_component(EXAMPLE_NAME ${EXAMPLE_SOURCE} NAME_WE)
    add_executable(${EXAMPLE_NAME} ${EXAMPLE_SOURCE})
    target_link_libraries(${EXAMPLE_NAME} print)
    install(TARGETS ${EXAMPLE_NAME}
      RUNTIME DESTINATION bin
    )
  endforeach(EXAMPLE_SOURCE ${EXAMPLE_SOURCES})
endif()
install(TARGETS print
    EXPORT print-config
    ARCHIVE DESTINATION lib
    LIBRARY DESTINATION lib
)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/ DESTINATION include)
install(EXPORT print-config DESTINATION cmake)
cmake -H. -B_build -DCMAKE_INSTALL_PREFIX=_install
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.10 will be removed from a future version of
  CMake.
  Update the VERSION argument <min> value.  Or, use the <min>...<max> syntax
  to tell CMake that the project requires at least <min> but has been updated
  to work with policies introduced by <max> or earlier.
-- Configuring done (0.0s)
-- Generating done (0.0s)
-- Build files have been written to: /Users/sam/samchik7/workspace/projects/lab03/_build
cmake --build _build --target install
[100%] Built target print
Install the project...
-- Install configuration: ""
-- Installing: /Users/sam/samchik7/workspace/projects/lab03/_install/lib/libprint.a
-- Installing: /Users/sam/samchik7/workspace/projects/lab03/_install/include
-- Installing: /Users/sam/samchik7/workspace/projects/lab03/_install/include/print.hpp
-- Installing: /Users/sam/samchik7/workspace/projects/lab03/_install/cmake/print-config.cmake
-- Installing: /Users/sam/samchik7/workspace/projects/lab03/_install/cmake/print-config-noconfig.cmake
tree _install
_install
├── cmake
│   ├── print-config-noconfig.cmake
│   └── print-config.cmake
├── include
│   └── print.hpp
└── lib
    └── libprint.a



git add CMakeLists.txt
git commit -m"added CMakeLists.txt"
[main 28cdff2] added CMakeLists.txt
 1 file changed, 36 insertions(+)
 create mode 100644 CMakeLists.txt
git push origin main
 git push origin main  
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 1.84 KiB | 1.84 MiB/s, done.
Total 7 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/samchik7/lab03.git
   28cdff2..025870b  main -> main.













v
