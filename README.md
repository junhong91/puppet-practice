# puppet-practice 📌

## Installing puppet 🤖

### 1. Enable the Puppet platform on Apt

root로 접속 후, 아래 명령어 수행

```
wget https://apt.puppet.com/puppet7-release-focal.deb
sudo dpkg -i puppet7-release-focal.deb
```

apt 패키지 리스트 업데이트 수행

```
sudo apt-get update
```

### 2. Install Puppet Server

Puppet Server를 구동하기 위해, JVM(Java Virtual Machine) 필요

puppet 패키지 설치

```
sudo apt-get install puppetserver
```

puppet 서비스 실행

```
sudo systemctl start puppetserver
```

`PATH` 환경 변수 업데이트

```
bash -l
```

정상적으로 설치 되었는지 확인

```
puppetserver -v
```
