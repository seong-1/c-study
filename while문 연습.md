# c-study

#include<stdio.h>

int main() {
	int num, i = 1, sum = 0, count = 0;

	scanf_s("%d", &num);
	//구구단
	while (i < 10) {
		printf("%d x %d = %d\n", num, i, num * i);
		i++;
	}
	//평균구하기
	while (num != 0) {//0을 입력받으면 종료
		sum += num;
		count++;
		scanf_s("%d", &num);
	}
	printf("평균 = %.2f", (float)sum / count);
	//수의 입력을 정수로 받았기에 소수점까지 받기위해 float 형식으로 변환

	return 0;
}
