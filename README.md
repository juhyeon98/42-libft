# Libft
## 소개
- 42 커리큘럼의 첫번째 과제이며, 자주 사용되는 C 표준 라이브러리 함수들을 직접 구현하는 프로젝트입니다.
- 그리고 구현한 함수들은 정적 라이브러리로 컴파일되도록 하여 이후의 과제에서도 사용될 수 있도록 구성되어 있습니다.

## 주요 기능
| 함수 시그니처 | 함수 기능 | 반환 값 |
|---------------|-----------|----------|
| `int ft_isalpha(int ch)` | `ch`가 알파벳인지 판별 | 참(1) 혹은 거짓(0) |
| `int ft_isdigit(int ch)` | `ch`가 숫자인지 판별 | 참(1) 혹은 거짓(0) |
| `int ft_isalnum(int ch)` | `ch`가 알파벳 또는 숫자인지 판별 | 참(1) 혹은 거짓(0) |
| `int ft_isascii(int ch)` | `ch`가 ASCII 코드 범위인지 판별 | 참(1) 혹은 거짓(0) |
| `int ft_isprint(int ch)` | `ch`가 출력 가능한 문자인지 판별 | 참(1) 혹은 거짓(0) |
| `size_t ft_strlen(const char *str)` | 문자열 길이를 반환 | 문자열 길이 |
| `void *ft_memset(void *str, int ch, size_t len)` | 메모리를 `ch` 값으로 채움 | 채워진 메모리 주소 |
| `void ft_bzero(void *str, size_t len)` | 메모리를 0으로 초기화 | 없음 |
| `void *ft_memcpy(void *dst, const void *src, size_t len)` | `src` 내용을 `dst`로 복사 (겹치면 안 됨) | `dst` 주소 |
| `void *ft_memmove(void *dst, const void *src, size_t len)` | `src` 내용을 `dst`로 복사 (겹쳐도 됨) | `dst` 주소 |
| `size_t ft_strlcpy(char *dst, const char *src, size_t d_size)` | `src`를 `dst`에 복사 | 복사한 길이 |
| `size_t ft_strlcat(char *dst, const char *src, size_t d_size)` | `src`를 `dst` 뒤에 붙임 | 최종 문자열 길이 |
| `int ft_toupper(int ch)` | 문자를 대문자로 변환 | 변환된 문자 |
| `int ft_tolower(int ch)` | 문자를 소문자로 변환 | 변환된 문자 |
| `char *ft_strchr(const char *str, int ch)` | 문자열에서 `ch`의 첫 위치 찾기 | 해당 주소 또는 `NULL` |
| `char *ft_strrchr(const char *str, int ch)` | 문자열에서 `ch`의 마지막 위치 찾기 | 해당 주소 또는 `NULL` |
| `int ft_atoi(const char *str)` | 문자열을 정수로 변환 | 변환된 정수 |
| `void *ft_calloc(size_t count, size_t size)` | 초기화된 메모리 할당 | 메모리 주소 |
| `char *ft_strdup(const char *str)` | 문자열 복사 (새 공간에) | 복사된 문자열 |
| `char *ft_substr(char const *s, unsigned int start, size_t len)` | 부분 문자열 추출 | 복사된 문자열 |
| `char *ft_strjoin(char const *s1, char const *s2)` | 문자열 합치기 | 합쳐진 문자열 |
| `char *ft_strtrim(char const *s1, char const *set)` | 양쪽에서 `set`에 해당하는 문자 제거 | 잘라낸 문자열 |
| `char **ft_split(char const *s, char c)` | 구분자 `c`로 문자열 분할 | 문자열 배열 |
| `char *ft_itoa(int n)` | 정수를 문자열로 변환 | 문자열 |
| `char *ft_strmapi(char const *s, char (*f)(unsigned int, char))` | 함수 `f`를 적용한 새 문자열 생성 | 새 문자열 |
| `void ft_striteri(char *s, void (*f)(unsigned int, char*))` | 문자열 각 문자에 함수 `f` 적용 | 없음 |
| `void ft_putchar_fd(char c, int fd)` | 문자 출력 (파일 디스크립터 사용) | 없음 |
| `void ft_putstr_fd(char *s, int fd)` | 문자열 출력 | 없음 |
| `void ft_putendl_fd(char *s, int fd)` | 문자열 출력 + 개행 | 없음 |
| `void ft_putnbr_fd(int n, int fd)` | 정수 출력 | 없음 |
| `t_list *ft_lstnew(void *content)` | 새 리스트 노드 생성 | 새 노드 |
| `void ft_lstadd_front(t_list **lst, t_list *new)` | 리스트 앞에 노드 추가 | 없음 |
| `void ft_lstadd_back(t_list **lst, t_list *new)` | 리스트 뒤에 노드 추가 | 없음 |
| `int ft_lstsize(t_list *lst)` | 노드 개수 반환 | 개수 |
| `t_list *ft_lstlast(t_list *lst)` | 마지막 노드 반환 | 마지막 노드 또는 `NULL` |
| `void ft_lstdelone(t_list *lst, void (*del)(void *))` | 노드 삭제 및 해제 | 없음 |
| `void ft_lstclear(t_list **lst, void (*del)(void *))` | 리스트 전체 삭제 | 없음 |
| `void ft_lstiter(t_list *lst, void (*f)(void *))` | 각 노드에 함수 `f` 적용 | 없음 |
| `t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *))` | 함수 `f` 적용한 새 리스트 반환 | 새 리스트 |
## 문제 해결점
### 문자열 처리
  - `ft_strjoin` 이나 `ft_split`과 같이 문자열 자체를 처리하는 과정에서 언제나 Segmentation fault가 나지 않도록 주의해야 했다.
  - 문자열 처리에서 Segmentation fault가 나는 이유는 문자열의 index가 문자열 범위를 벗어나는 경우이다.
  - 문자열이 유효한지(제대로 메모리에 할당되었는지), 문자열이 할당된 메모리 공간을 벗어나 참조하려는 것은 아닌지 반드시 확인해야 한다.
### 메모리 관리
  - 리스트 관련 함수 등에서 할당한 메모리를 해제할 때, 꼼꼼하게 해제해야만 한다.
  - 리스트 노드에 저장되어 있는 데이터를 먼저 해제하고, 노드를 해제해야한다.
### 함수의 선조건과 후조건
  - 함수의 선조건과 후조건을 모두 만족해야 한다.
  - 함수의 선조건을 만족시키기 위해, 매개변수의 유효성을 검사했다.
    - 특히나 포인터의 경우, `NULL`인지 아닌지 판단을 해야 한다.
  - 함수의 후조건을 만족시키기 위해, 원본 함수의 결과값과 비교하며 구현했다.
    - 가장 난해했던 것이 `atoi`였으며, 실제 Unix에서 제공하는 `atoi`의 결과 값을 분석하여 후조건이 만족할 수 있도록 구현했다.
    - `atoi`에서는 `+`와 `-`를 모두 인식하며, 숫자가 아닌 문자가 올때까지만 해석한다.
    - 그리고 그 결과가 `int`범위를 넘어서는 경우 오버플로우가 된다.
