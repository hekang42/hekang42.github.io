get_next_line의 흔적

-. fd(file descriptor) 의 최대값  -> limits.h / OPEN_MAX

0. OPEN(FILE)
GNL
1. s = READ(BUFFER_SIZE)
2. CHECK_NEW_LINE(s)
2-1. strjoin -> READ AGAIN
2-2. strjoin -> return
     NEW_LINE 뒷 부분 저장 -> temp(static)
GNL
3. temp + READ(BUFFER_SIZE)
반복 2.
