* 파일 구조
```
AnsibleVulnScanner
├── playbooks/
│   ├── main.yml                   # 메인 플레이북
│   ├── linux_servers.yml           # 리눅스 서버 플레이북
│   ├── windows_servers.yml         # 윈도우 서버 플레이북
├── roles/
│   ├── linux_role/                 # 리눅스 역할 디렉터리
│   │   ├── tasks/
│   │   │   ├── main.yml            # 리눅스용 작업 정의
│   │   ├── vars/
│   │   │   ├── main.yml            # 리눅스용 변수 정의
│   ├── windows_role/               # 윈도우 역할 디렉터리
│   │   ├── tasks/
│   │   │   ├── main.yml            # 윈도우용 작업 정의
│   │   ├── vars/
│   │   │   ├── main.yml            # 윈도우용 변수 정의
```
* 플레이북 실행
```
ansible-playbook playbooks/main.yml
```
