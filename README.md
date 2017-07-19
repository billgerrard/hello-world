# Hello World in various programming languages I've used

## BASIC

    10 PRINT "HELLO WORLD"

## Pascal

    program HelloWorld;

    begin
        writeln('Hello World');
    end.

## Assembly

    dosseg
    .model small
    .stack 100h

    .data
    hello_message db 'Hello, World!',0dh,0ah,'$'

    .code
    main  proc
    mov ax,@data
    mov ds,ax

    mov ah,9
    mov dx,offset hello_message
    int 21h

    mov ax,4C00h
    int 21h
    main  endp
    end main

## C

    #include <stdio.h>
    #include <stdlib.h>

    int main(void)
    {
        printf("Hello, world\n");
        return EXIT_SUCCESS;
    }

## C++

    #include <iostream>

    int main()
    {
        std::cout << "Hello, World.";
        return 0;
    }

## BBx

## ProvideX

    begin
        print "Hello World!"
    end

## Perl

    print "Hello World\n"

## Python

    print "hello world"

## Java

    public class HelloWorld {

        public static void main(String[] args) {
            System.out.println("Hello, World");
        }

    }
