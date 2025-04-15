# KLib2-Python

![Demo](img/KLib2_python_Demo.png)

A Python-based client library for connecting and processing sensor data from Snowforce 3.  
Supports real-time acquisition over TCP/IP, buffering, parsing, and simple terminal visualization.

> This code is provided as an example. Actual performance may vary depending on system configuration.

---

## Features

- TCP/IP-based client interface
- Real-time ADC data parsing
- Dynamic detection of row/column structure in packets
- Lightweight and easy to run
- Max FPS(Frames per second) : 30

---

## Development Environment

- [Python 3.9](https://www.python.org)
- [NumPy](https://numpy.org/install/)
- Snowforce 3  
  [Download Link](https://github.com/kitronyx/snowforce3/blob/master/Snowforce3.0_2022.02.17.exe)

---

## Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/kitronyx/klib2-python.git
cd klib2-python
```

### 2. Install required packages

```bash
pip install numpy
```

### 3. Run the sample client

```bash
python klib2-python.py
```

### 4. Expected Output

- Sensor data displayed in a matrix format

---

## Code Overview

### `KLib` Class

This class contains the core logic for TCP/IP communication and data processing.

| Method             | Description |
|--------------------|-------------|
| `__init__`         | Initializes connection variables and buffers |
| `init()`           | Establishes socket connection and parses the initial packet |
| `read()`           | Reads a full packet and updates the ADC buffer |
| `printadc()`       | Prints the ADC matrix to the console |
| `start()` / `stop()` | Starts or closes the TCP/IP socket connection |

---

## Contact

For technical support or inquiries,  
please visit **https://www.kitronyx.com/support_request** or contact your representative.

---

# KLib2-Python

![Demo](img/KLib2_python_Demo.png)

Python 기반의 클라이언트 라이브러리로, Snowforce 3에서 센서 데이터를 연결하고 처리할 수 있습니다.  
TCP/IP를 통한 실시간 수집, 버퍼링, 파싱, 간단한 터미널 시각화를 지원합니다.

> 본 코드는 예제 용도로 제공되며, 실제 성능은 시스템 환경에 따라 달라질 수 있습니다.

---

## 주요 특징

- TCP/IP 기반 클라이언트 인터페이스
- 실시간 ADC 데이터 파싱
- 동적으로 행/열을 감지하는 패킷 처리
- 가볍고 실행이 간편함
- 최대 통신 속도 30 FPS(Frame per second)

---

## 개발 환경

- [Python 3.9](https://www.python.org)
- [NumPy](https://numpy.org/install/)
- Snowforce 3  
  [다운로드 링크](https://github.com/kitronyx/snowforce3/blob/master/Snowforce3.0_2022.02.17.exe)

---

## 퀵스타트

### 1. 저장소 클론

```bash
git clone https://github.com/kitronyx/klib2-python.git
cd klib2-python
```

### 2. 필수 패키지 설치

```bash
pip install numpy
```

### 3. 샘플 클라이언트 실행

```bash
python klib2-python.py
```

### 4. 실행 시 출력 예시

- 센서 데이터가 행렬 형태로 출력됨

---

## 코드 개요

### `KLib` 클래스

TCP/IP 통신 및 데이터 처리의 핵심 로직이 포함된 클래스입니다.

| 메서드            | 설명 |
|------------------|------|
| `__init__`       | 연결 변수 및 버퍼 초기화 |
| `init()`         | 소켓 연결 수립 및 첫 패킷 파싱 |
| `read()`         | 전체 패킷을 읽고 ADC 버퍼 업데이트 |
| `printadc()`     | ADC 행렬을 콘솔에 출력 |
| `start()` / `stop()` | 소켓 연결 시작 및 종료 |

---

## 문의

기술 지원 또는 문의는  
**https://www.kitronyx.co.kr/support_request** 를 방문하거나 담당자에게 문의해 주세요.
