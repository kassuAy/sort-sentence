# sort-sentence
class Solution:
    def sortSentence(self, s: str) -> str:
        words = s[::-1].split()
        result = [word[1:][::-1] for word in sorted(words)]
        return ' '.join(result)
