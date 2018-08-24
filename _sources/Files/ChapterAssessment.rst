..  Copyright (C)  Brad Miller, David Ranum, Jeffrey Elkner, Peter Wentworth, Allen B. Downey, Chris
    Meyers, and Dario Mitchell.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

.. qnum::
   :prefix: files-10-
   :start: 1

Chapter Assessment
==================

.. datafile:: travel_plans.txt
   :hide:

   This summer I will be travelling.
   I will go to...
   Italy: Rome
   Greece: Athens
   England: London, Manchester
   France: Paris, Nice, Lyon
   Spain: Madrid, Barcelona, Granada
   Austria: Vienna
   I will probably not even want to come back! 
   However, I wonder how I will get by with all the different languages.
   I only know English!

.. datafile:: school_prompt.txt
   :hide:

   Writing essays for school can be difficult but
   many students find that by researching their topic that they
   have more to say and are better informed. Here are the university
   we require many undergraduate students to take a first year writing requirement
   so that they can
   have a solid foundation for their writing skills. This comes
   in handy for many students.
   Different schools have different requirements, but everyone uses
   writing at some point in their academic career, be it essays, research papers,
   technical write ups, or scripts.

1. The textfile, ``travel_plans.txt``, contains the summer travel plans for someone with some commentary. Find the total number of characters in the file and save to the variable ``num``.

.. activecode:: ac9_10_1

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(num, 316, "Testing that num value is assigned to correct value.")

   myTests().main()

2. We have provided a file called ``emotion_words.txt`` that contains lines of words that describe emotions. Find the total number of words in the file and assign this value to the variable ``num_words``.

.. activecode:: ac9_10_2

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(num_words, 48, "Testing that num_words was assigned to the correct value.")

   myTests().main()

3. Assign to the variable ``num_lines`` the number of lines in the file ``school_prompt.txt``.

.. activecode:: ac9_10_3

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(num_lines, 10, "Testing that num_lines has the correct value.")

   myTests().main()

4. Assign the first 30 characters of ``school_prompt.txt`` as a string to the variable ``beginning_chars``.

.. activecode:: ac9_10_4

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(len(beginning_chars), 30, "Testing that beginning_chars has the correct length.")
         self.assertEqual(beginning_chars, "Writing essays for school can ", "Testing that beginning_chars has the correct string.")

   myTests().main()   

5. **Challenge:** Using the file ``school_prompt.txt``, assign the third word of every line to a list called ``three``.

.. activecode:: ac9_10_5

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(three, ['for', 'find', 'to', 'many', 'they', 'solid', 'for', 'have', 'some', 'ups,'], "Testing that three has the correct value.")

   myTests().main()

6. **Challenge:** Create a list called ``emotions`` that contains the first word of every line in ``emotion_words.txt``. 

.. activecode:: ac9_10_6

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(emotions, ['Sad', 'Angry', 'Happy', 'Confused', 'Excited', 'Scared', 'Nervous'], "Testing that emotions was created correctly.")

   myTests().main() 


7. Assign the first 33 characters from the textfile, ``travel_plans.txt`` to the variable ``first_chars``.

.. activecode:: ac9_10_7

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testFive(self):
         self.assertEqual(first_chars, "This summer I will be travelling.", "Testing that first_chars is assigned to correct value.")

   myTests().main()

8. **Challenge:** Using the file ``school_prompt.txt``, if the character 'p' is in a word, then add the word to a list called ``p_words``.

.. activecode:: ac9_10_8

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(p_words, ['topic', 'point', 'papers,', 'ups,', 'scripts.'], "Testing that p_words has the correct list.")

   myTests().main()
