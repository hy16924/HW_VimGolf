# HW_VimGolf

## (1) Add quotes to ansible playbook
 ### $ vimgolf put 5f0f5fbe280fbf000c233304

![vimgolf(1)](https://user-images.githubusercontent.com/66362763/144480739-00af1643-256a-4e5a-880c-0f8840e7e35d.gif)

G(파일의 마지막 줄로 이동) -> W(단어 시작점으로 이동) -> i(현재 위치에서 insert mode) -> "  입력 

-> end(문자열 끝으로이동) -> " 입력 -> esc(일반 모드로)-> ctrl+ZZ(종료)

![image](https://user-images.githubusercontent.com/66362763/144481219-73351fe4-b76d-40ee-9d41-cb0939db6f3e.png)

## (2) simple replacements
### $ vimgolf put 603ba26a01b4d00009c10a49

![vimgolf_2](https://user-images.githubusercontent.com/66362763/144597080-511cedfb-2e56-4328-9582-af8a8dca9a96.gif)

w(단어 앞으로 이동) -> dw(현재 단어 끝까지 자라내기) -> i(현재 위치에서 insert mode) -> vim 입력 -> <esc>(일반 모드)

-> :(명령행 모드) -> %s/emacs/vim/g (전체에서 문자열 "emacs"를 "vim"으로 바꾸기) -> ctrl+ZZ(종료)

![vimgolf_2_result](https://user-images.githubusercontent.com/66362763/144597594-8c9d5700-f0c3-4a66-90d8-d6ef5f2e1c5d.png)

## (3) Satisfy the go linter
### $ vimgolf put 5f1063aa8361810006e73210
  
![vimgolf_3](https://user-images.githubusercontent.com/66362763/144610128-3c647f84-bd8e-46b9-93d3-4a4528d210b8.gif)
  
 5+G(5번째 행으로 이동) -> V(라인 비주얼 모드) + 방향키<up> -> y(복사) -> p(붙여넣기) -> :norm i// (//입력, 주석처리)
  
 -> 6+G(6번째 행으로 이동) -> .(dot)(마지막 동작 반복) -> w(단어 이동) -> dw(현재 단어 삭제) -> a(현재 위치 다음 칸에서 입력 모드)
  
 -> "TODO"입력 -> <esc>(일반 모드로) -> b(단어 뒤로) -> yw(단어복사, TODO) ->  p(붙여넣기, 4번째 행 Version 뒤) 
  
  -> dw(단어 삭제, string) -> ctrl+ZZ(종료)

 ![vimgolf_3_result](https://user-images.githubusercontent.com/66362763/144610135-85035d12-38d9-4663-9f92-c2dbf841e778.png)
 
## (4) Plotting some variables in python
### $ vimgolf put 9v0060da5177000000000209
  
 ![vimgolf_4](https://user-images.githubusercontent.com/66362763/144660874-310ad841-31da-49c9-a472-5289effee857.gif)
  
 ?k(위쪽으로 단어(k) 검색) -> r(한 글자만 바꾸기)+'g'/'r'/'b'(k를 g,r,b로) -> :%s/y1/abs(y1)(문자열 교체, y1->abs(y1)으로)
  
 -> { (단락 단위 이동, 앞쪽으로) -> ?1(위쪽으로 단어(1) 검색) -> r + '4'/'3'/'2'(1을 2,3,4로) -> .(dot)(마지막 동작 반복) 
  
 -> ctrl+ZZ(종료)
  
 ![vimgolf_4_result](https://user-images.githubusercontent.com/66362763/144660891-c0303dbd-dabd-432d-931e-655f131d7dcb.png)
 
## (5) Python dataclasses
### $ vimgolf put 6013804df3308e0009368f1c

 ![vim_golf5](https://user-images.githubusercontent.com/66362763/144660938-798df14c-5f49-4882-85f1-5989a1f1e410.gif) 
  
 5G(5번째 행으로 이동) -> V(비주얼 라인 모드) -> < (내어쓰기) -> :5,8s/:.*/, (5행부터 8행까지에 한해서 ':' 이후 모두를 ','로 대체)
  
 -> i(insert mode) -> ...  -> Home(행의 처음으로) -> yy(현재 라인 복사) -> u(ctrl+z, 되돌리기) -> G(파일의 마지막으로 이동)  
  
  -> end(행의 마지막으로) -> ... -> p(붙여넣기) -> ... ctrl+ZZ(종료)

 ![vimgolf_5_result](https://user-images.githubusercontent.com/66362763/144660944-771c852c-9baf-4f18-ad18-7b0b5dbf06e4.png)

