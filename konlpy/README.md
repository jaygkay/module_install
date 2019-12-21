### konlpy 모듈 설치하기 (Mac 기준)

#### 1. xcode 없을 시에 설치하기

`$ xcode-select --install`

#### 2. JAVA SE 없을 시에 설치하기

- 2019.12 기준 최신 버전
  - https://www.oracle.com/technetwork/java/javase/downloads/jdk13-downloads-5672538.html

`$ /usr/libexec/java_home`

/Library/Java/JavaVirtualMachines/jdk-10.0.2.jdk/Contents/Home

`$ cat >> ~/.bash_profile`

export JAVA_HOME=$(/usr/libexec/java_home)

`^C`

`$ source ~/.bash_profile`

`$ echo $JAVA_HOME`

/Library/Java/JavaVirtualMachines/jdk-10.0.2.jdk/Contents/Home

#### 3. JPype와 konlpy 동시 설치
`$ export MACOSX_DEPLOYMENT_TARGET=10.10`

`$ CFLAGS='-stdlib=libc++' pip install konlpy`

