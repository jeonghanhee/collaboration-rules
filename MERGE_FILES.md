# MERGE_FILES
이 문서는 혼자서 개발하는 것이 아니라 여러 사람들이서 협업을 할 때 필수로 지켜야하는 문서입니다.

### 각자 역할을 구분하여 영역을 나누세요.
- 어떤 사람은 `UI` 폴더만 고치고, 어떤 사람은 `Gameplay` 이런식으로 게임 내에서의 기능 및 유지보수를 담당해야 합니다.
- 위 경우는 사실 별개로 Merge(병합)을 할 때는 복잡한 상황이 발생하지 않습니다. 그러므로 그대로 푸시해도 상관 없습니다.

### 그러나 여러 사람들의 영역이 겹친다면?
- `Merge` 폴더를 하나 생성합니다. 그리고 수정한 스크립트 파일들은 복사하여 이 폴더에 넣으세요. 만약 다른 사람이 이미 수정한 동일 파일이 있다면 두 파일 간의 차이를 검사합니다. 겹치는 부분이 있다면 어떤 부분을 넣을건지 서로 합의를 합니다. 그렇게 합의된 부분은 폴더에 그대로 반영합니다.
- 위 과정을 거친뒤 `Merge`에 있는 모든 파일들을 그대로 `Scripts` 폴더에 반영합니다.
- 단, 파일을 그대로 `Merge` 폴더에 넣지말고 서브 디렉토리 내부에 넣어야 합니다. (예시: UIManager는 `Merge/UI` 안에)