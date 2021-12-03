# HW_VimGolf

![vimgolf(1)](https://user-images.githubusercontent.com/66362763/144480739-00af1643-256a-4e5a-880c-0f8840e7e35d.gif)

G(파일의 마지막 줄로 이동) -> W(단어 시작점으로 이동) -> i(현재 위치에서 insert mode) -> "  입력 

-> end(문자열 끝으로이동) -> " 입력 -> esc(일반 모드로)-> ctrl+ZZ(나가기)

![image](https://user-images.githubusercontent.com/66362763/144481219-73351fe4-b76d-40ee-9d41-cb0939db6f3e.png)

![vimgolf_2](https://user-images.githubusercontent.com/66362763/144597080-511cedfb-2e56-4328-9582-af8a8dca9a96.gif)

w(단어 앞으로 이동) -> dw(현재 단어 끝까지 자라내기) -> i(현재 위치에서 insert mode) -> vim 입력 -> <esc>(일반 모드)

-> :(명령행 모드) -> %s/emacs/vim/g (전체에서 문자열 "emacs"를 "vim"으로 바꾸기) -> ctrl+ZZ(나가기)

![vimgolf_2_result](https://user-images.githubusercontent.com/66362763/144597594-8c9d5700-f0c3-4a66-90d8-d6ef5f2e1c5d.png)

![vimgolf_3](https://user-images.githubusercontent.com/66362763/144610128-3c647f84-bd8e-46b9-93d3-4a4528d210b8.gif)
  
 5+G(5번째 행으로 이동) -> V(라인 비주얼 모드) + 방향키<up> -> y(복사) -> p(붙여넣기) -> :norm i// (//입력, 주석처리)
  
 -> 6+G(6번째 행으로 이동) -> .(dot)(마지막 동작 반복) -> w(단어 이동) -> dw(현재 단어 삭제) -> a(현재 위치 다음 칸에서 입력 모드)
  
 -> "TODO"입력 -> <esc>(일반 모드로) -> b(단어 뒤로) -> yw(단어복사, TODO) ->  p(붙여넣기, 4번째 행 Version 뒤) -> dw(단어 삭제, string) 
  
 -> ctrl+ZZ(나가기)

![vimgolf_3_result](https://user-images.githubusercontent.com/66362763/144610135-85035d12-38d9-4663-9f92-c2dbf841e778.png)
  
  ![vimgolf_4](https://user-images.githubusercontent.com/66362763/144660874-310ad841-31da-49c9-a472-5289effee857.gif)

  ![vimgolf_4_result](https://user-images.githubusercontent.com/66362763/144660891-c0303dbd-dabd-432d-931e-655f131d7dcb.png)

  ![vim_golf5](https://user-images.githubusercontent.com/66362763/144660938-798df14c-5f49-4882-85f1-5989a1f1e410.gif)

  ![vimgolf_5_result](https://user-images.githubusercontent.com/66362763/144660944-771c852c-9baf-4f18-ad18-7b0b5dbf06e4.png)

