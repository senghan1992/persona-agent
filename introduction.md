# Persona Agent

## Data gathering

- 특정 인물에 대한 정보 수집

- data gathering pipeline architecture
    - 영상 data -> 음성 분리 -> 화자 분리 -> text 화 -> RAG
    - 텍스트 data -> RAG
    - 음성 data -> 화자 분리 -> text 화 -> RAG

- 자원 문제 -> 고려대학교 연구실 자원 빌려서 사용

## Agent Layer Architecture

- 현재 여러 agent framework들이 나오면서 여러 방향의 agent layer 방법론들이 거론되고 있는데 어느하나 아직 standard라고 부르기 애매합니다. 이럴때 이런 layer 구조를 활용해서 구축해보려고 하는데 우려되는 부분이 있으신지 궁금합니다.

- 할루시네이션을 모든 케이스에 대해 잡는게 어려울 듯 한데 어떤식으로 필터링을 거는지?

- performance 체크에 대해서는 어떻게 해야 하는지? 모든 것에 정답을 두고 performance를 체크할 수는 없을 것 같음

- manager agent
    - persona picker agent
    - persona agent
    - legal issue agent
    - performance check agent (prompt 성능 체크) persona-estimator

- 기본 persona 별 prompt
    - 각 사용자별 prompt

## Agent ops

- AgentOps : 에이전트의 효율적인 운영에 특화

- RAGOps : 검색(retreival) 및 생성(generation) 프로세스를 포함하는 RAG 솔루션을 효율적으로 운영하는데 중점을 둔다

- PromptOps : 프롬프트 저장, 관리 및 최적화를 포함하여 프롬프트를 효과적으로 운영하는데 중점을 둔다