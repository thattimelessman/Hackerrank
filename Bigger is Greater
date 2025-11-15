def biggerIsGreater(w):
    l = [*w]
    if l == sorted(l, reverse=True):
        return 'no answer'
    for j in range(1, len(l)):
        for i in range(j):
            #Find which character to swap.
            if l[-i-1] > l[-j-1]:
                #Swap characters.
                l[-i-1], l[-j-1] = l[-j-1], l[-i-1]
                #Sort characters that follow swapped character.
                l = l[:-j] + sorted(l[-j:])
                return ''.join(l)
              
              
              
              
              
