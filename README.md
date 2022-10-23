# 카운터에 거스름돈으로 사용할 500원, 100원, 50원, 10원 동전이 무한히 존재한다고 가정할 때 거스름돈은 n, 거슬러줘야 할 동전의 최소 개수 구하기

n = int(input("거스름 돈을 입력하세요"))
count = 0

coin_types = [500, 100, 50, 10]

for coin in coin_types:
  count += n // coin
  n %= coin
print(count)
