# MINI_LIB

The extended data type structure for vanilla C language

**Disclaimer:** This code is for learning purpose, using with prudence in production. Owner does *NOT* guarantee the quality of this code.

## Naming convention

**CamelCase**

1. Type

Any new type should be treated as reference type. 

    Ex: NewType, HashMap, ...

Long type can be shortened. 

    Ex: SingleLinkedList -> Sll, ...
2. Function

Functions of mini_lib usually provide support for a new defined type. Thus, their names should indicate the associate type.

    Ex: newTypeAction like hashMapPut, ...

There are 2 name types of function actionType, typeAction.

1. If Type is the main type (HashMap, SLL) and function return that type, we use action+TypeName.

        Ex: createHashMap, initHashMap, ...

1. If return type is subtype (SingleLinkedNode), we use mainType+Action+Subtype.

        Ex: sllCreateNode, ...

1. If function does modify internal values of DataType, we use typeName+Action.

        Ex: hashMapGet

3. File

    Types and functions declaration should be grouped in my_type.h and function description should be in my_type.c
