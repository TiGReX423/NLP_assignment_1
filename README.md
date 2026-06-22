# Assignment 1

Small FST that represents morphology fragment of my native language:
- language: Russian
- FST fragment: feminine nouns of the 1st declension (`-а` / `-я`)
- coverage goal: full singular and plural case paradigm for a small noun set
- words in the current draft: `берёза`, `книга`, `башня`, `вишня`, `кухня`

Files:
- `assignment_1_hfst.ipynb` - starter notebook
- `russian_feminine_nouns.lexc` - lexicon and paradigm definitions

What is already included:
- full case tags for noun generation
- three rule types required by the task:
  - insertion: fleeting vowel in genitive plural (`башня -> башен`, `вишня -> вишен`)
  - substitution: spelling rule `ы -> и` after velars/hushing consonants (`книга -> книги`, because `берёза -> берёзы`)
  - removal: cleanup of technical morphophonemic markers
- one more complex case:
  - exception-like genitive plural `кухня -> кухонь`
