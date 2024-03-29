### 자바스크립트에서 얕은 복사(Shallow Copy)와 깊은 복사(Deep Copy)에 대해 설명해 주세요.

먼저 shallow Copy는 얕은 복사라고 불리며, 원본 객체를 복사하는데 내부의 객체와 배열에도 영향을 미치는 복사입니다.

오리지널 배열과 얕은 복사를 한 배열이 있을 때, 복사된 배열의 내부를 수정하면 똑같이 오리지널 배열에도 영향이가 
내부가 바뀌게 됩니다.

그리고 Deep Copy는 깊은 복사라고 불리며, 원본 객체의 모든 속성을 본따서 그대로 새로운 객체를 생성하는 복사입니다.

오리지널 배열과 똑같이 생긴 새로운 배열을 만든 것이기 때문에, 깊은 복사 배열의 내부를 수정해도 오리지널 배열에
영향이 가지 않습니다.

### var, let, const 를 중복 선언 허용, 스코프, 호이스팅 관점에서 서로 비교해 주세요.

1. 중복 선언

var는 중복 선언이 가능해서 나중에 선언한 값으로 값이 덮어씌워집니다.
let은 같은 스코프 내에서 같은 변수명으로 중복 선언이 허용되지 않습니다.
const는 상수라고 지칭하며, 한번 선언한 값은 변경할 수 없습니다.

2. 스코프

var는 함수 내에서 선언된 변수는 함수 내에서만 유효하며, 블록 스코프를 무시합니다.
let과 const는 블록 스코프를 가지고 있어서, 블록 내에서 선언된 변수는 블록 내에서만 유효합니다.

3. 호이스팅

var는 호이스팅이 발생하며 변수가 선언되기 전에도 참조할 수 있습니다. 다만 초기화되지 않은 변수는 'undefined'로 초기화 됩니다.

let과 const는 호이스팅이 발생이 한다고는 하지만 변수를 초기화하지 않아서 에러가 발생합니다.