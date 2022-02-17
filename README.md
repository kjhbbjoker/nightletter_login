# 항해99 미니프로젝트 8조 - 나의 우체국📮
- 넘치는 sns! 하지만 고요한 밤에 누군가에게 날리는 편지는 더욱 의미있겠죠? 나만의 우체국이 되어드립니다. 다들 편지하세요~!
<img width="129" alt="스크린샷 2022-02-17 오전 10 34 11" src="https://user-images.githubusercontent.com/89513776/154388794-0c8fe607-7ac0-4812-a2aa-5ea16b5a6a53.png">

[나의 우체국을 구경해보세요!](http://letter99.s3-website.ap-northeast-2.amazonaws.com/)

#### 프론트 - [안진희](https://github.com/YJ-my),[최예진](https://github.com/YJ-my)
#### 백 - [이승민](https://github.com/howCanIFind),[김종훈](https://github.com/kjhbbjoker),[신동석](https://github.com/dss1222)

#### 프론트 GIT-HUB 주소 https://github.com/YJ-my/sparta-w6-letter

<hr/>

### API 설계서
https://www.notion.so/anggom/8-585643bae5aa47bc813e57ff8e5a9fcd


### 와이어프레임

<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/0007e0cc-91c2-422f-911f-31eecab220b1/%E1%84%86%E1%85%B5%E1%84%82%E1%85%B5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3_%E1%84%8B%E1%85%AA%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%A5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%86%B7_1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T013937Z&X-Amz-Expires=86400&X-Amz-Signature=3fa1b589c116a1d573ca247320f101128e27df9a8f81305ee06dd23438d46e8a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E1%2584%2586%25E1%2585%25B5%25E1%2584%2582%25E1%2585%25B5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A6%25E1%2586%25A8%25E1%2584%2590%25E1%2585%25B3%2520%25E1%2584%258B%25E1%2585%25AA%25E1%2584%258B%25E1%2585%25B5%25E1%2584%258B%25E1%2585%25A5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A6%25E1%2584%258B%25E1%2585%25B5%25E1%2586%25B7%25201.png%22&x-id=GetObject" width="500px">

<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/2e02933e-1b01-43dc-bffa-f0c9ecd99121/%E1%84%86%E1%85%B5%E1%84%82%E1%85%B5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3_%E1%84%8B%E1%85%AA%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%A5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%86%B7_2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014022Z&X-Amz-Expires=86400&X-Amz-Signature=1ac26d21ebe486924ad021001e28cad7e619c240dd370b2e98de6ea3eb465145&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E1%2584%2586%25E1%2585%25B5%25E1%2584%2582%25E1%2585%25B5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A6%25E1%2586%25A8%25E1%2584%2590%25E1%2585%25B3%2520%25E1%2584%258B%25E1%2585%25AA%25E1%2584%258B%25E1%2585%25B5%25E1%2584%258B%25E1%2585%25A5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A6%25E1%2584%258B%25E1%2585%25B5%25E1%2586%25B7%25202.png%22&x-id=GetObject" width="500px">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/36baff97-ad7d-4863-9d36-f85ffd07a992/%EB%AF%B8%EB%8B%88%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8_%EC%99%80%EC%9D%B4%EC%96%B4%ED%94%84%EB%A0%88%EC%9E%84_3.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014118Z&X-Amz-Expires=86400&X-Amz-Signature=ef4fcc8b26f0d1f476104b2d5aa2fe809878baddcc3ab1e7a8f89d186c402df8&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25EB%25AF%25B8%25EB%258B%2588%25ED%2594%2584%25EB%25A1%259C%25EC%25A0%259D%25ED%258A%25B8%2520%25EC%2599%2580%25EC%259D%25B4%25EC%2596%25B4%25ED%2594%2584%25EB%25A0%2588%25EC%259E%2584%25203.png%22&x-id=GetObject" width="500px">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/adf63276-57ae-46b8-8123-e26526f9390e/%E1%84%86%E1%85%B5%E1%84%82%E1%85%B5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3_%E1%84%8B%E1%85%AA%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%A5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%86%B7_5.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014131Z&X-Amz-Expires=86400&X-Amz-Signature=2289ff5d0aca1ff200397c8b89386c0209b80a240ef72d6509fa5dafbf431752&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E1%2584%2586%25E1%2585%25B5%25E1%2584%2582%25E1%2585%25B5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A6%25E1%2586%25A8%25E1%2584%2590%25E1%2585%25B3%2520%25E1%2584%258B%25E1%2585%25AA%25E1%2584%258B%25E1%2585%25B5%25E1%2584%258B%25E1%2585%25A5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A6%25E1%2584%258B%25E1%2585%25B5%25E1%2586%25B7%25205.png%22&x-id=GetObject" width="500px">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/adf63276-57ae-46b8-8123-e26526f9390e/%E1%84%86%E1%85%B5%E1%84%82%E1%85%B5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3_%E1%84%8B%E1%85%AA%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%A5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%86%B7_5.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014144Z&X-Amz-Expires=86400&X-Amz-Signature=8f4f5f8aba3208d2a7f0f0922ef0b1ed47b04f3d3a3276c539afbf48c47138c9&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E1%2584%2586%25E1%2585%25B5%25E1%2584%2582%25E1%2585%25B5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A6%25E1%2586%25A8%25E1%2584%2590%25E1%2585%25B3%2520%25E1%2584%258B%25E1%2585%25AA%25E1%2584%258B%25E1%2585%25B5%25E1%2584%258B%25E1%2585%25A5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A6%25E1%2584%258B%25E1%2585%25B5%25E1%2586%25B7%25205.png%22&x-id=GetObject" width="500px">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/89e7a659-93dd-44c7-bb95-1822131aaeb4/%EB%AF%B8%EB%8B%88%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8_%EC%99%80%EC%9D%B4%EC%96%B4%ED%94%84%EB%A0%88%EC%9E%84_4.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014153Z&X-Amz-Expires=86400&X-Amz-Signature=c3ff8d7a536fb96e9fdf471c7da92adef1461f0a2cb4d5ae00732eb410c5c4d0&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25EB%25AF%25B8%25EB%258B%2588%25ED%2594%2584%25EB%25A1%259C%25EC%25A0%259D%25ED%258A%25B8%2520%25EC%2599%2580%25EC%259D%25B4%25EC%2596%25B4%25ED%2594%2584%25EB%25A0%2588%25EC%259E%2584%25204.png%22&x-id=GetObject" width="500px">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3d8a92cb-073f-472d-9a3e-251bfdada1c2/%E1%84%86%E1%85%B5%E1%84%82%E1%85%B5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3_%E1%84%8B%E1%85%AA%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%A5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%86%B7_8.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014208Z&X-Amz-Expires=86400&X-Amz-Signature=c238c7cd7e83f49e6b98dd5e2ecfb52259e7e6579811c7502c1fc1cf89333958&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E1%2584%2586%25E1%2585%25B5%25E1%2584%2582%25E1%2585%25B5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A6%25E1%2586%25A8%25E1%2584%2590%25E1%2585%25B3%2520%25E1%2584%258B%25E1%2585%25AA%25E1%2584%258B%25E1%2585%25B5%25E1%2584%258B%25E1%2585%25A5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A6%25E1%2584%258B%25E1%2585%25B5%25E1%2586%25B7%25208.png%22&x-id=GetObject" width="500px">
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/de734aba-742f-4279-a3b7-7390065063db/%E1%84%86%E1%85%B5%E1%84%82%E1%85%B5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3_%E1%84%8B%E1%85%AA%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%A5%E1%84%91%E1%85%B3%E1%84%85%E1%85%A6%E1%84%8B%E1%85%B5%E1%86%B7_6.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220217%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220217T014239Z&X-Amz-Expires=86400&X-Amz-Signature=3acb21ac9b44c3541678c9019d6f924d4399d1faf3229806957867a0ea053bf4&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E1%2584%2586%25E1%2585%25B5%25E1%2584%2582%25E1%2585%25B5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A9%25E1%2584%258C%25E1%2585%25A6%25E1%2586%25A8%25E1%2584%2590%25E1%2585%25B3%2520%25E1%2584%258B%25E1%2585%25AA%25E1%2584%258B%25E1%2585%25B5%25E1%2584%258B%25E1%2585%25A5%25E1%2584%2591%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25A6%25E1%2584%258B%25E1%2585%25B5%25E1%2586%25B7%25206.png%22&x-id=GetObject" width="500px">


### Entity Relatuonship Diagram
<img src="https://user-images.githubusercontent.com/97422693/154409375-b7475703-869e-4ccd-b082-d3c5fdaa8111.PNG" width="500px">



###Trouble Shooting


<details>
<summary>JSON형식이 아닌 FORM 데이터 형식으로 넘어가는 오류 발생</summary>
<div markdown="1">

```java
@PutMapping("/api/posts/{postId}")
    public void editLetter(@PathVariable Long postId,
                              @RequestBody PostsRequestDto requestDto) {
        postsService.editLetter(requestDto,postId);
    }
```
@RequestBody을 사용하지 않아서 발생하는 문제임을 확인하고 해결

</div>
</details>







<details>
<summary>게시물 삭제 시 댓글이 있을 경우 테이블 연관 관계로 인해 자식 테이블을 삭제 못함으로 인해 삭제 안되는 문제 발생</summary>
<div markdown="1">


```java
public boolean deleteLetter(Long postId) {
        Posts posts = postsRepository.findById(postId).orElseThrow(
                () -> new NullPointerException("해당 게시물이 존재하지 않습니다.")
        );
        List<Reply> replys = replyRepository.findAllByPosts(posts);
        for (Reply reply : replys) {
            replyRepository.deleteById(reply.getId());
        }
        postsRepository.deleteById(postId);
        return true;
    }
```
cascade를 이용하여 해결하는 법도 있엇지만 서비스 게시물 Delete로직에서  자식 테이블인 댓글을 먼저 모두 삭제 시킨 다음에 게시물을 삭제 되게 로직을 수정함으로 해결


</div>
</details>




<details>
<summary>백엔드와 프론트 Request 요청 시에 발생하는 오류들</summary>
<div markdown="1">




```java
logging.level.org.apache.coyote.http11: debug
```
클라이언트가 보낸 요청 메시지 로그 보는 방법인 logging.level.org.apache.coyote.http11: debug을 이용하여 문제를 찾으면서 해결

</div>
</details>
    
    
    
<details>
<summary>서버 과부하 최소화를 위한 성능 최적화 작업</summary>
<div markdown="1">




..........

</div>
</details>





