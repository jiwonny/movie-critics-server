# MAD CRITICS

평론가들의 영화 평론과 평점을 한번에 보고 싶어 진행한 프로젝트. 국내 및 해외 영화 평론 사이트에서 평론가들의 평론 및 기타 정보들을 가져와 웹사이트 구성.

<b><i>Front: Vue.js, Back: Python, Node.js, Database: PostgreSQL</i></b>
[Front Repository](https://github.com/jiwonny/movie-critics-front)
[Server Repository](https://github.com/jiwonny/movie-critics-server)

<br>

### 구성
- Main : 2 sections 로 분리되어 있음. 첫번째 section 은 현재 개봉작의 순위를 보여주고 두번째 section 은 개봉 예정작의 목록을 보여줌.
- 영화 목록 Tab : 개봉 예정작, 현재 개봉작, 기타 영화 목록을 구분해서 볼 수 있음. 
- 장르별 영화 Tab : 여러 장르별로 구분해놓은 영화 목록을 볼 수 있음.

#### <i>영화 목록 Display 방식</i>
- 영화 포스터 및 영화 정보를 포함.
- 네이버 및 해외 영화 평론 사이트에서 <b>평론가들이 준 평점</b> 만을 모아 영화 평점 표시.

#### <i>영화 Detail Page</i>
- 영화 기본적인 정보를 비롯하여 줄거리, 예고편 동영상으로 이동할 수 있는 url 등을 표시.
- 네이버와 해외 영화평론 사이트인 Rotten Tomato, MetaCritic 에서 영화 평론가들이 남긴 평론을 보여줌
- 각 사이트에서 평론가들이 영화에 부여한 평점을 평균내어 표시

<br>

### 데이터베이스 구축
- `Python`을 이용해 <b>크롤러</b> 만듦
- 크롤링을 이용해 네이버 영화 사이트에 있는 영화들을 기준으로 영화 데이터베이스 구축
- 크롤링을 이용해 Rotten Tomato 와 Movie Critic 에서 데이터베이스 내에 있는 영화가 있는지 확인하여 평론 및 평점을 데이터베이스에 추가

<br>

