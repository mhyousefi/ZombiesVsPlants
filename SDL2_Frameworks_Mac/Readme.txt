1-Copy .framework files into your library directory (/Library/Frameworks/)
2-Replace your rsdl.hpp with the file included
3-use -framework option to include these frameworks
  g++ rsdl.cpp demo1.cpp -framework SDL2 -framework SDL2_image -framework SDL2_ttf
