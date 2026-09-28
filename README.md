# comp3353
assignment

Xu Yihang
3036389737
U3638973@connect.hku.hk

``
path = input()

a = 0
c = 0
g = 0
t = 0

file = open(path, "r")
for line in file:
    # skip the header lines
    if line.startswith(">"):
        continue
    for ch in line:
        ch = ch.upper()
        if ch == "A":
            a = a + 1
        elif ch == "C":
            c = c + 1
        elif ch == "G":
            g = g + 1
        elif ch == "T":
            t = t + 1
file.close()

print(a, c, g, t)
``
