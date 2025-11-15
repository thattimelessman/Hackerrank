def gridlandMetro(n,m,k,track):
    occupied,log=0,{}
    for i in track:
        if i[0] not in log:
            log[i[0]]=[i[1],i[2]]
            occupied+=i[2]-i[1]+1
        else:
            l,r=log[i[0]][0],log[i[0]][1]
            if i[1]<=r:
                if i[2]>r:
                    log[i[0]]=[l,i[2]]
                    occupied+=i[2]-r
            else:
                log[i[0]]=[i[1],i[2]]
                occupied+=i[2]-i[1]+1
    return n*m-occupied
