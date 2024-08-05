# 웹 스터디

1주차
+ xss 취약점 실습 환경 만들기
  + reflected, stored, DOM-based 발생하는 환경 구현

memo : th:text 사용시 HTML 엔티티로 변환되어 span 태그 내에서 출력됨

---

2주차
+ Secure Coding
+ CSP
  + 인라인 스크립트와 외부 스크립트 출처를 제한
  + 외부 자원 로딩을 제한
  + 의도하지 않은 콘텐츠 실행 방지

  + 이번에 적용한 내용
    + default-src 'self': 기본적으로 모든 리소스는 현재 도메인에서만 로드
    + script-src 'self': 스크립트는 현재 도메인에서만 로드
    + object-src 'none': <object>, <embed>, <applet> 태그를 통한 콘텐츠 로드를 차단
    + style-src 'self': 스타일 시트는 현재 도메인에서만 로드
    + img-src 'self': 이미지는 현재 도메인에서만 로드
  + self: 현재 웹 페이지와 동일한 출처를 의미