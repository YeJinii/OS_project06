# OS_project06
파일 시스템

* 과제 목표
  - 가상 디스크(애뮬레이터)를 위한 간단한 파일 시스템 및 기본 파일 operation 구현
  - 디스크 접근 기능이 구현된 ssufs-disk.h와 ssufs-disk.c에서 정의(구현된)된 여러 함수를 이용하여, ssufs-ops.c를 수정(ssufs_create(), ssufs_delete(), ssufs_read(), ssufs_write() 구현)

* 기본 지식
  - 가상 디스크
  - inode 구조체
  - ssu_disk.c에 구현된 함수 설명

* 과제 기본 내용
  - 기본 지식에서 설명한 함수를 이용하여 과제 구현 내용의 기능 구현 (ssufs-ops.h 확인 및 ssufs-ops.c 수정)
  - ssu-disk.h : file handle 배열이라고 하는 메모리 내 데이터 구조를 정의함
  - Linux 및 Unix 시스템과 달리 create()와 open()은 별도로 구현

* 과제 구현 내용
  1. int ssufs_create(char * filename)
  2. void ssufs_delete(char * filename)
  3. int ssufs_open(char * filename)
  4. void ssufs_close(int file handle)
  5. int ssufs_read(int file handle, char * buf, int nbytes)
  6. int ssufs_write(int file handle, char * buf, int nbytes)
  7. int ssufs_lseek(int file handle, int nseek)
