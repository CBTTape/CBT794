# CBT794
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 794 is from Daniel F. Gaeta and contains a useful REXX    *   FILE 794
//*           function, called RXMEM.                               *   FILE 794
//*                                                                 *   FILE 794
//*           email:  dfgaeta@br.ibm.com                            *   FILE 794
//*                                                                 *   FILE 794
//*    Description:                                                 *   FILE 794
//*                                                                 *   FILE 794
//*    I am a Rexx lover and the RXMEM is one more function         *   FILE 794
//*    from my personal library that I would like to share          *   FILE 794
//*    with you.                                                    *   FILE 794
//*                                                                 *   FILE 794
//*    As I work with other languages, like Java, VB, Pascal        *   FILE 794
//*    and C++, sometimes I need to use linked list, in Java        *   FILE 794
//*    for example, ArrayList class...                              *   FILE 794
//*                                                                 *   FILE 794
//*    That is an interesting technique to manage items from a      *   FILE 794
//*    list, using to resources like insert, add to end, count      *   FILE 794
//*    items, delete items and other.                               *   FILE 794
//*                                                                 *   FILE 794
//*    Now I am provinding the first version of RXMEM.              *   FILE 794
//*                                                                 *   FILE 794
//*    The RXMEM has the following features :                       *   FILE 794
//*      - to manage token pair service, using IEANTxx modules      *   FILE 794
//*      - to manage getmain and freemain memory                    *   FILE 794
//*      - to manage linked list options                            *   FILE 794
//*                                                                 *   FILE 794
//*    As I am working on improvements, I am not delivering         *   FILE 794
//*    the source code.  Just a rexx samples.                       *   FILE 794
//*                                                                 *   FILE 794
//*    Please, let me know about possible abends and issues.        *   FILE 794
//*                                                                 *   FILE 794
//*    Gaeta, Daniel                                                *   FILE 794
//*    IBM/BR                                                       *   FILE 794
//*                                                                 *   FILE 794
//*    This is a summary of function/actions :                      *   FILE 794
//*                                                                 *   FILE 794
//*                                                                 *   FILE 794
//*      FUNCTION  : RXMEM                                          *   FILE 794
//*      PARAMETER : RXMEM(ACTION,LISTNAME,<..>)                    *   FILE 794
//*                                                                 *   FILE 794
//*      ACTIONS   :                                                *   FILE 794
//*        TKCRT - CREATE A TOKEN PAIR                              *   FILE 794
//*        RET=('TKCRT',PAIR1,PAIR2)                                *   FILE 794
//*        ...                                                      *   FILE 794
//*        TKDEL - DELETE A TOKEN PAIR                              *   FILE 794
//*        RET=('TKDEL',PAIR1)                                      *   FILE 794
//*        ...                                                      *   FILE 794
//*        TKRTV - RETRIEVE A TOKEN PAIR                            *   FILE 794
//*        RET=('TKRTV',PAIR1)                                      *   FILE 794
//*        ...                                                      *   FILE 794
//*        OBTAIN - OBTAIN MEMORY USING BYTES                       *   FILE 794
//*        ADR=('OBTAIN',D2C(<BYTES>,4))                            *   FILE 794
//*        ...                                                      *   FILE 794
//*        RELEASE - RELEASE MEMORY OBTAINED FROM OBTAIN            *   FILE 794
//*        RET=('RELEASE',D2C(<ADDR>,4),D2C(<LEN>,4))               *   FILE 794
//*        ...                                                      *   FILE 794
//*        CREATE - CREATE A NEW LINKED LIST                        *   FILE 794
//*        RET=('CREATE',<LNAME>)                                   *   FILE 794
//*        ...                                                      *   FILE 794
//*        DESTROY - DESTROY PREVIOUS LINKED LIST CREATED           *   FILE 794
//*        RET=('DESTROY',<LNAME>)                                  *   FILE 794
//*        ...                                                      *   FILE 794
//*        ADD - ADD AN ELEMENT INTO END OF LIST                    *   FILE 794
//*        RET=('ADD',<LNAME>,<STR>)                                *   FILE 794
//*        ...                                                      *   FILE 794
//*        DEL - DELETE AN ELEMENT IN ORDINAL POSITION              *   FILE 794
//*        RET=('DEL',<LNAME>,D2C(<POS>,4))                         *   FILE 794
//*        ...                                                      *   FILE 794
//*        GET - GETTING A DATA ITEM FROM ORDINAL POSITION          *   FILE 794
//*        STR=('GET',<LNAME>,D2C(<POS>,4))                         *   FILE 794
//*        ...                                                      *   FILE 794
//*        SET - SETTING A DATA ITEM TO ORDINAL POSITION            *   FILE 794
//*        STR=('SET',<LNAME>,D2C(<POS>,4),<STR>)                   *   FILE 794
//*        ...                                                      *   FILE 794
//*        COUNT - NUMBER ELEMENTS FROM LINKED LIST                 *   FILE 794
//*        CNT=('COUNT',<LNAME>)                                    *   FILE 794
//*        ...                                                      *   FILE 794
//*        SAVESTEM - UPDATE STEM VARIABLE WITH ITEMS FROM LIST     *   FILE 794
//*        RET=('SAVESTEM',<LNAME>)                                 *   FILE 794
//*        ...                                                      *   FILE 794
//*        LOADSTEM - UPDATE ITEMS FROM LIST USING STEM VARIABLE    *   FILE 794
//*        RET=('LOADSTEM',<LNAME>,D2C(<BEGIN>,4),D2C(<END>,4))     *   FILE 794
//*        ...                                                      *   FILE 794
//*        INS - INSERT AN ELEMENTO IN ORDINAL POSITION             *   FILE 794
//*        RET=('INS',<LNAME>,D2C(<POS>,4),<STR>)                   *   FILE 794
//*                                                                 *   FILE 794
```
