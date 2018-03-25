---
layout: post
title:  "유용한 Rust 관련 사이트 모음"
tags:   ["Rust"]
published: true
---

수 년 동안 [Rust][] 프로그래밍을 하면서 참고해 오고 있는 사이트들을 간단히 정리해 보았습니다. 주로 중급 단계 이상으로 올라가는 데에 도움이 될 만한 내용을 담고 있거나, 앞으로의 변화를 따라가기에 유용한 곳들이라고 생각합니다.

Rust가 처음이시거나 아직 생소한 분께는 먼저 [Rust by Example](https://rustbyexample.com/)을 읽으시면서 예제 코드를 직접 따라해보시는 것을 추천드리겠습니다. 😊


# [This Week in Rust](https://this-week-in-rust.org/)

한 주 사이에 올라온 Rust 관련 소식이 정리되어 올라오는 사이트입니다. Rust 뉴스 및 새로운 블로그 글을 확인하는 용도로도 충분히 유용하지만, 특히 아래에서 언급할 Rust RFC의 진행 상황을 한눈에 보기 좋습니다. 어쩌면 Rust 관련 행사 소식에 관심이 있으신 분이 계실지도 모르겠네요.
매주 수요일에 업데이트됩니다.


# [Docs.rs](https://docs.rs/)

[Cargo 패키지 저장소](https://crates.io/)에 올라오는 패키지에 대한 레퍼런스 문서가 이 곳에 자동으로 올라옵니다. 특이한 라이브러리가 아닌 이상 이 곳에서 대부분의 라이브러리 레퍼런스를 찾을 수 있습니다. 소스 코드 저장소나 관련 홈페이지를 찾고 싶을 때도 괜찮은 출발점이 될 수 있습니다.


# [Serde](https://serde.rs/)

Rust에서 [JSON][]이나 [TOML][], [CBOR][] 등 여러 종류의 직렬화 데이타 형식을 읽고 쓰는 데에 널리 사용되는 라이브러리입니다. 간편하게 원하는 구조체에 간단한 선언을 붙여 주는 것만으로 사용 가능한 것은 물론, 넓은 범위의 커스터마이징이 가능하며 필요할 경우 데이타를 복사 없이 읽는 것도 얼마든지 가능합니다. 2018년에 JSON이나 이와 비슷한 데이타를 다루지 않을 일은 거의 없을 테니, 자세한 사용법에 익숙해져서 손해 볼 일이 없습니다.


# [The Rustonomicon](https://doc.rust-lang.org/nomicon/)

[이름이 굉장히 무시무시한][1] 이 문서는 Rust 언어의 어두운 구석들, 가령 초기화되지 않은 메모리나 메모리 누수, 자세한 수명(lifetime) 규칙, 강제 타입 변환 등 평범한 Rust 프로그래밍의 범주를 넘어가기 시작할 때 알아두면 좋을 내용을 다루고 있습니다. 특히 C 라이브러리를 호출하는 코드를 직접 작성해야 하거나, 새로운 동기화 도구를 만들거나, 효율적인 자료 구조를 구현하기 위해 타입 시스템을 우회하고 싶을 때처럼 본격적으로 `unsafe`와 친해지게 될 시점에 읽어 두시는 것을 추천합니다.


# [The Unstable Book](https://doc.rust-lang.org/nightly/unstable-book/)

Rust 나이틀리 컴파일러에서만 쓸 수 있는 [기능 플래그][feature flag]의 모든 목록을 참조할 수 있는 문서입니다. [`conservative_impl_trait`](https://doc.rust-lang.org/nightly/unstable-book/language-features/conservative-impl-trait.html)처럼 널리 쓰이는 기능의 경우 간단한 부연 설명이 붙어 있는 경우도 있어서, 앞으로 추가될 기능을 간단히 둘러보거나 처음 보는 기능 플래그의 사용법을 찾을 때 유용합니다.


# [Rust RFCs](https://github.com/rust-lang/rfcs/pulls)

Rust 언어 및 표준 라이브러리와 기타 개발 도구에 대한 개선 제안이 올라오는 곳입니다. [Python Enhancement Proposals][PEP] (PEP)와 비슷하게 Rust 커뮤니티의 의견을 모으고 내용을 정돈해서 공식화하는 역할을 담당하므로, 앞으로 Rust가 어떻게 변화할지를 이곳을 통해 따라갈 수 있습니다. RFC 제출 및 승인 프로세스는 GitHub 풀 리퀘스트를 통해 진행되며, RFC 번호 또한 풀 리퀘스트의 이슈 번호로 정해집니다. 이미 채택된 RFC 문서들은 [이곳](https://rust-lang.github.io/rfcs/)에서 좀 더 편하게 열람할 수 있습니다.


[Rust]: https://www.rust-lang.org/
[JSON]: https://www.json.org/
[TOML]: https://github.com/toml-lang/toml
[CBOR]: http://cbor.io/
[1]: https://ko.wikipedia.org/wiki/%EB%84%A4%ED%81%AC%EB%A1%9C%EB%85%B8%EB%AF%B8%EC%BD%98
[feature flag]: https://doc.rust-lang.org/nightly/book/second-edition/appendix-07-nightly-rust.html#unstable-features
[PEP]: https://www.python.org/dev/peps/
