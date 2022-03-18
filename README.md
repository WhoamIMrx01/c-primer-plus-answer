
#include <stdio.h>

int main()
{
	printf("请输入时间以分钟为单位：\n");
	const int danwei = 60;
	int minute=1;
	//scanf_s("%d", &minute);
	int hour, min;
	while (minute > 0) {
		scanf_s("%d", &minute);

		if (minute >= danwei) {
		hour = minute / danwei;
		min = minute - danwei * hour;
		printf("%d分钟是%d小时%d分钟\n", minute, hour, min);
		}

		else if (minute>0)
			printf("%d分钟是%d分钟\n",minute,minute);
		
		
	}
if (minute == 0)
			printf("0分钟没有定义哦");
		else
			printf("你搁这开玩笑了");



	return 0;
}
