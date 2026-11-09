# 안녕하세요. 정명훈입니다. 👋

**디지털 회로 설계·검증과 임베디드 시스템**을 공부하고 있습니다.
RTL 설계부터 UVM 검증, FPGA 구현, MCU 펌웨어까지 하드웨어와 소프트웨어가 접목되는 부분을 설계 및 검증하는 과정을 업로드하였습니다.

## 🛠 Tech Stack

| 분야 | 기술 |
|---|---|
| HDL / 검증 | SystemVerilog, Verilog, UVM |
| 임베디드 | C, STM32 HAL, I2C / UART / PWM / EXTI / Timer |
| AI / Vision | Python, YOLO11 · YOLO26, OpenCV, TFLite (LiteRT), NCNN, Raspberry Pi |
| Tools | Synopsys VCS · Verdi, Xilinx Vivado, STM32CubeIDE, Git |
| Board | Digilent Basys3 (Artix-7), STM32 NUCLEO-F411RE |

## 📌 Projects

### Digital Design & Verification

| 프로젝트 | 설명 | 핵심 |
|---|---|---|
| [**RV32I Multi-Cycle CPU + APB**](https://github.com/wjdaudgns120-max/rv32i-cpu-project) | RISC-V RV32I 멀티사이클 CPU와 APB 버스(BRAM/GPI/GPO) 설계, C 코드를 기계어로 실행해 검증 | SystemVerilog · APB · UVM · 4인 팀 |
| [**FIFO UVM Verification**](https://github.com/wjdaudgns120-max/verificate-fifo-used-uvm) | 동기 FIFO를 UVM 테스트벤치로 검증, 스코어보드 fail 0 · coverage 100% | UVM · Scoreboard · Coverage |
| [**Basys3 UART Watch & Sensor**](https://github.com/wjdaudgns120-max/basys3-uart-watch-sensor) | 시계·스톱워치·DHT11·HC-SR04를 FPGA로 구현하고 UART 명령으로 제어, 타이밍 위반(WNS −5.487ns → +0.016ns) 해결 | Verilog · FSM · UART · Timing |

### Embedded

| 프로젝트 | 설명 | 핵심 |
|---|---|---|
| [**STM32 Smart Watch**](https://github.com/wjdaudgns120-max/stm32_smartwatch) | 버튼 하나로 시계·온습도·거리·스톱워치를 전환하는 스마트 워치, App→Service→Driver 계층 구조 | STM32 HAL · I2C LCD · RTC · 이벤트 큐 |
| [**STM32 Analog Clock**](https://github.com/wjdaudgns120-max/stm32_analog_timeclock_project) | 스텝 모터 3개로 시·분·초침을 구동하는 아날로그 시계, 타이머 인터럽트 기반 목표 추종과 탈조 해결 | Step Motor · TIM 인터럽트 · RTC · 4인 팀 |
| [**Card-Access Hotel Elevator**](https://github.com/wjdaudgns120-max/STM32_Elevator_Project) | 카드 권한으로 갈 수 있는 층을 제한하는 3층 호텔 엘리베이터. SCAN 스케줄러와 2-process FSM으로 운행하고, Python GUI와 8바이트 UART 프레임으로 문 핸드셰이크 · 응답 검증 | SCAN 스케줄러 · FSM · UART 프로토콜 · Python GUI · 2인 팀 |

### AI / Vision

| 프로젝트 | 설명 | 핵심 |
|---|---|---|
| [**CNN RPS Game**](https://github.com/wjdaudgns120-max/CNN_RPSGAME_Project) | 웹캠으로 두 사람의 손을 탐지해 가위바위보 승패를 실시간 판정, YOLO 출력 디코딩·NMS 직접 구현 | YOLO11n · TFLite · OpenCV |
| [**CNN Door Counter (Team)**](https://github.com/wjdaudgns120-max/CNN_Team_Project) | 라즈베리파이 4대로 출입문 영상을 분산 처리해 드나드는 사람 수를 실시간으로 세는 시스템. 카메라 Pi가 프레임을 작업자 Pi 2대에 부하 분산하고, 결과를 모아 추적 · IN/OUT 판정 · 웹으로 표시 | YOLO26s-seg (NCNN) · ByteTrack · TCP 분산 처리 · Flask · 팀 프로젝트 |

## 📫 Contact

- GitHub: [@wjdaudgns120-max](https://github.com/wjdaudgns120-max)
