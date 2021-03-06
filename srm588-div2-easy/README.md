

Problem Statement

     You are exploring a dungeon. In the dungeon you found some locked doors. Each
     locked door has some red and some green keyholes (zero or more of each kind).
     In order to open a door, you must insert fitting keys into all its keyholes
     simultaneously. Once you open a door, you may take all the keys back and
     possibly reuse some of them later to open other doors.
     There are three kinds of keys: red, green, and white ones. Each red key fits
     into any red keyhole. Each green key fits into any green keyhole. Each white
     key fits into any keyhole (both red and green ones).
     You are given int[]s doorR and doorG. These two int[]s have the same length.
     For each valid i, the values doorR[i] and doorG[i] describe one of the doors
     you found: a door with doorR[i] red and doorG[i] green keyholes.
     You are also given the int[] keys with three elements: keys[0] is the number of
     red keys, keys[1] the number of green keys, and keys[2] the number of white
     keys you have at the beginning.
     Return the number of doors you can open with keys you have.

Definition


     Class:            KeyDungeonDiv2
     Method:           countDoors
     Parameters:       int[], int[], int[]
     Returns:          int
     Method signature: int countDoors(int[] doorR, int[] doorG, int[] keys)
     (be sure your method is public)

    

Constraints

  -  doorR and doorG will each contain between 1 and 50 elements, inclusive.
  -  doorR and doorG will contain the same number of elements.
  -  Each element of doorR and doorG will be between 0 and 100, inclusive.
  -  keys will contain exactly 3 elements.
  -  Each element of keys will be between 0 and 100, inclusive.

Examples

 0)



       {2, 0, 5, 3}


       {1, 4, 0, 2}


       {2, 3, 1}



       Returns: 3
    

     There are 4 doors. You have 2 red keys, 3 green keys, 1 white key. You can
     open 3 of the doors:

     * You can open door 0, using 2 red keys and 1 green key.
     * You can open door 1, using 3 green keys and 1 white key. Here you insert
       the white key into one of the green keyholes.
     * You can't open door 2, for you have only 3 keys that can be inserted into
       red key holes.
     * You can open door 3, using 2 red keys, 2 green keys, and 1 white key. Here
       you insert the white key into one of the red keyholes.



 1)



       {0, 1, 2, 0}


       {0, 2, 3, 1}


       {0, 0, 0}



       Returns: 1


     You have no key at all, but door 0 also has no keyhole. Therefore, you
     can open door 0.


 2)



       {3, 5, 4, 2, 8}


       {4, 2, 3, 8, 1}

    
       {0, 0, 10}



       Returns: 5




 3)



       {4, 5, 4, 6, 8}


       {2, 1, 2, 3, 5}

    
       {1, 2, 1}



       Returns: 0




 4)



       {41,44,41,57,58,74,84,100,58,2,43,32,82,97,44,13,35,98,96,81,43,77,18,51,27,
        27,39,39,45,82,59,20,28,93,6,39,64,78,28,85,17,56,3,68,4,0,36,80,41,77}


       {67,15,53,36,88,29,26,57,68,99,97,27,51,70,3,49,65,75,35,92,66,0,23,96,38,86,
        98,31,26,75,30,2,92,78,100,99,38,26,85,74,77,15,16,48,100,88,55,93,99,54}
    

       {39,31,34}



       Returns: 17





This problem statement is the exclusive and proprietary property of TopCoder,
Inc. Any unauthorized use or reproduction of this information without the prior
written consent of TopCoder, Inc. is strictly prohibited. (c)2003, TopCoder,
Inc. All rights reserved.
