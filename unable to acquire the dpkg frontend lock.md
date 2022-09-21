## 1. 문제(Problem)

리눅스에서 apt를 통해 'htop' 프로그램을 설치하는 도중 에러가 발생했다.

![문제](https://user-images.githubusercontent.com/54324782/191628855-b29ce9ad-e22a-4fda-8c83-5ae94044ee1b.png)


------------------


## 2. 해결(Solved)

####   - 모든 프로세스 종료
```bash
sudo killall apt apt-get
```

![1](https://user-images.githubusercontent.com/54324782/191628917-96bf9522-a95a-49c3-8e7d-da93ed00b990.png)

####   - 위와 같이 진행 중인 프로세스가 없다고 한다면, 아래 세 가지의 디렉토리 삭제
```bash
sudo rm /var/lib/apt/lists/lock
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock*
```

####   - 업데이트 수행
```bash
sudo dpkg --configure -a

sudo apt update
```

![3](https://user-images.githubusercontent.com/54324782/191628957-2a26f209-090b-48c5-b254-b37c0dd7bad1.png)
