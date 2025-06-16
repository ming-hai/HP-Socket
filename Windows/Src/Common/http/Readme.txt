http_parser Modifications
--------------------
1. move 'enum state' from http_parser.cpp to http_parser.h
2. http_parser.h ignore warning: 4005
3. http_parser.cpp ignore warning: 4018,4456

llhttp Modifications
--------------------
1. llhttp_api.c ignore warning: 4715
2. llhttp_url.c ignore warning: 4456
3. llhttp_internal.c ignore warning: 4244, 4152, 4055, 4702
4. llhttp_url.h : LLHTTP_STRICT_MODE set default value 1
5. llhttp.h : delete codes below
    #elif defined(_WIN32)
    #define LLHTTP_EXPORT __declspec(dllexport)