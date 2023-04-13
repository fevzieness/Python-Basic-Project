# Python-Basic-Project

l = [[1, 'a', ['cat'], 2], [[[3]], 'dog'], 4, 5]
l1 = []

def flatten(l):

    for i in l:
        if isinstance(i, list):
            flatten(i)
        else:
            l1.append(i)

flatten(l)
print(l1)


l = [[1, 2], [3, 4], [5, 6, 7]]

def new_list(l):
    for i in l:
        i.reverse()
    l.reverse()
    return(l)
    
new_list(l)
  
