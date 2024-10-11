#----------------------------------------------------------------------
# 1. criar lista 2d A 3x4 com todos os elementos com valor 1
#----------------------------------------------------------------------
m = 3; n = 4
A = []
for i in range(m): A.append([1] * n)

print(A)

#----------------------------------------------------------------------
# 2. criar lista 2d B 5x4 com o 1o elemento = 1, o 2o = 2, etc., até o ultimo = 20
#----------------------------------------------------------------------
m = 5; n = 4
B = []
for i in range(m): B.append([0] * n) # cria toda zerada

# substitui os 0's pelos valores 1, 2, 3, ..., 20
x = 1
for i in range(m):
    for j in range(n):
        B[i][j] = x
        x += 1

print(B)

#----------------------------------------------------------------------
# 3. dada matriz quadrada C mxm, obter diagonal secundária
# (dica: indexação negativa... facilita muito! basta percorrer apenas as linhas)
#----------------------------------------------------------------------
C = [[1,2,3], [4,5,6], [7,8,9]] # matriz exemplo

# -- aqui começa o código pedido --
m = len(C)
diag_sec = []
for i in range(m):
    diag_sec.append(C[i][-(i+1)])

print(diag_sec)

#----------------------------------------------------------------------
# 4. seja uma matriz D, m x n, obter lista com a soma de cada coluna
#----------------------------------------------------------------------
D = [[1, 2], [10, 20], [100, 200]] # matriz exemplo

# -- aqui começa o código pedido --
m = len(D)
n = len(D[0])

soma_cols = [0] * n
# fazendo o for-j, for-i, podemos percorrer a matriz pelas colunas
# (para cada coluna, percorre-se todas as linhas)
for j in range(n):
    for i in range(m):
        soma_cols[j] += D[i][j]

print(soma_cols)
        
    



        