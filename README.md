파라미터 조정은 아래로 하면서 테스트 해봐야함

#define STEPPER_START_SPEED_HZ       200.0f

#define STEPPER_MAX_SPEED_HZ         1000.0f

#define STEPPER_ACCEL_HZ_PER_SEC     1000.0f


STEPPER_START_SPEED_HZ -> v0 즉 시작 종료 속도 설정. (초당 펄스 수)

STEPPER_MAX_SPEED_HZ -> 최고 속도 설정 (초당 펄스 수)

STEPPER_ACCEL_HZ_PER_SEC -> 가속도 (1초마다 초당 펄스 수 증가 즉 가속)

참고로 이 값들은 회전수가 기준이 아니고 STEP수 기준임.

대략 계산으로 1바퀴 돌려면 64000펄스 필요함.

수식은 등가속도 공식을 이용함.

추천값

100
1000
500
