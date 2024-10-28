* 파일 구조
```
AnsibleVulnScanner
├── playbooks/
│   ├── detec_os.yml                  # 버서 os 및 상태 확인 플레이북
│   ├── main.yml                      # 메인 플레이북
│   ├── linux_servers.yml             # 리눅스 서버 플레이북
│   ├── windows_servers.yml           # 윈도우 서버 플레이북
├── docs/
│   ├── server_inform.json            # 서버의 세부 내용 문서
│   ├── linux_checklist_detail.json   # 리눅스 취약점 항목 문서
│   ├── windows_checklist_detail.json # 윈도우 취약점 항목 문서
│   ├── linux_action_inform.json      # 리눅스 취약점 조치 문서
│   ├── windows_action_inform.json    # 윈도우 취약점 조치 문서
├── roles/
│   ├── linux_role/                   # 리눅스 역할 디렉터리
│   │   ├── tasks/
│   │   │   ├── main.yml              # 리눅스용 작업 정의
│   ├── windows_role/                 # 윈도우 역할 디렉터리
│   │   ├── tasks/
│   │   │   ├── main.yml              # 윈도우용 작업 정의
```
* 플레이북 실행
```
ansible-playbook playbooks/main.yml
```
