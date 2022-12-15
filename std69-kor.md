[본 파일은 한 개 이상의 RFC 문서를 취합한 파일입니다.]

네트워크 워킹 그룹 S. Hollenbeck
인터넷 주석 요청서(RFC): 5730 VeriSign, Inc.
STD: 69 2009년 8월
무효화: 4930
Category: Standards Track

# 확장성 프로비저닝 프로토콜 (EPP)

## 개요

본 포준에서는 공유된 중앙 저장소 상의 오브젝트의 프로비저닝 및 관리를 위한 어플리케이션 계층의 클라이언트-서버 프로토콜을 설명한다. 본 프로토콜은 XML로 지정되었으며 오브젝트 관리 작업 및 프로토콜 작업을 오브젝트로 연결하는 확장 가능한 프레임워크를 정의한다. 본 표준은 RFC 4930을 무효화한다.

## 본 문서의 상태

본 표준은 인터넷 공동체를 위한 인터넷 표준 추적 프로토콜을 명시하며, 개선을 위한 토론 및 제안을 요청한다. 본 프로토콜의 표준화 현황 및 상태를 확인하려면 "공식 인터넷 프로토콜 표준" (STD 1)의 최신판을 참고하도록 한다. 본 문서는 누구나 배포할 수 있다.

## 저작권 통지

Copyright (c) 2009 IETF Trust and the persons identified as the
document authors. All rights reserved.

This document is subject to BCP 78 and the IETF Trust's Legal
Provisions Relating to IETF Documents in effect on the date of
publication of this document (http://trustee.ietf.org/license-info).
Please review these documents carefully, as they describe your rights
and restrictions with respect to this document.

## 목차

1. 서론
   1.1. 본 표준에 사용된 규칙
2. 프로토콜 설명
   2.1. 전송 매핑 고려사항
   2.2. 프로토콜 설명
   2.3. 헬로(Hello) 형식
   2.4. 그리팅(Greeting) 형식
   2.5. 명령(Command) 형식
   2.6. 응답 형식
   2.7. 프로토콜 확장 프레임워크
   2.7.1. 프로토콜 확장
   2.7.2. 오브젝트 확장
   2.7.3. 명령-응답 확장
   2.8. 오브젝트 식별
   2.9. 프로토콜 명령
   2.9.1. 세션 관리 명렁
   2.9.1.1. EPP <login> 명령
   2.9.1.2. EPP <logout> 명령
   2.9.2. 쿼리 명령
   2.9.2.1. EPP <check> 명령
   2.9.2.2. EPP <info> 명령
   2.9.2.3. EPP <poll> 명령
   2.9.2.4. EPP <transfer> 쿼리 명령
   2.9.3. 오브젝트 변환 명령
   2.9.3.1. EPP <create> 명령
   2.9.3.2. EPP <delete> 명령
   2.9.3.3. EPP <renew> 명령
   2.9.3.4. EPP <transfer> 명령
   2.9.3.5. EPP <update> 명령
3. 결과 코드
4. 형식 구문
   4.1. 기본 스키마
   4.2. 공유 구조 스키마
5. 국제화 고려사항
6. IANA 고려사항
7. 보안 고려 사항
8. 사사
9. 참조
   9.1. 인용 표준
   9.2. 참고 표준

부록 A. 오브젝트 매핑 템플릿
부록 B. 미디어 유형 등록: application/epp+xml
부록 C. RFC 4930 변경 사항
