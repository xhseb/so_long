# so_long
## Summary

이 프로젝트는 매우 작은 2D 게임입니다. 질감, 스프라이트로 작업할 수 있도록 제작되었습니다. 그리고 기본적인 게임플레이 요소도 있습니다.

## Foreword

2D 게임의 경우 타일, 타일 세트, 스프라이트 및 스프라이트 시트를 검색해야 합니다.
고맙게도 일부 재능 있는 예술가들은 다음과 같은 플랫폼에서 기꺼이 작품을 공유합니다.
[itch.io](http://itch.io/)

## Constraints

- 운영 체제 또는 42seoul에서 제공하는 miniLibX를 사용해야 합니다. 소스로 사용하고 싶다면 위의 공통 지침 파트와 동일한 규칙을 libft에 적용해야 합니다.
- 다른 창으로 변경, 최소화 등 Window창 관리가 원활해야 합니다.
- 지도는 3개의 구성요소 walls, collectibles, free space으로 구성됩니다.
- 플레이어의 목표는 지도에 있는 모든 collectibles을 수집한 후 최소한의 움직임으로 탈출하는 것입니다.
- 움직일 때마다 쉘에 현재 이동 수가 표시되어야 합니다.
- 플레이어는 위, 아래, 왼쪽, 오른쪽을 움직일 수 있어야 합니다.
- 2D view (top-down or profile)를 사용합니다.
- 게임이 실시간일 필요는 없습니다.
- 플레이어가 wall으로 이동할 수 없습니다.
- 프로그램은 이미지를 Window창에 표시하고 다음 규칙을 따릅니다.

    ■ W, A, S, D 키를 사용하여 주인공을 이동합니다.

    ■ ESC를 누르면 윈도우가 닫히고 프로그램이 정상적으로 종료됩니다.

    ■ Window창의 빨간색 십자가를 클릭하면 창이 닫히고 프로그램을 깨끗이 종료합니다.

    ■ minilibX의 이미지 사용을 적극 권장합니다.

- 프로그램은 .ber 확장자를 가진 지도 파일을 첫 번째 인수로 사용해야 합니다.
■ 지도는 empty space 0, wall 1, collectibles C, map exit E, 플레이어의 시작 위치 P 등 5개의 문자로만 구성되어야 합니다.
- 지도는 벽으로 닫거나 둘러 쌓여야 합니다. 그렇지 않으면 프로그램에서 오류를 반환해야 합니다.
■ 지도에는 하나 이상의 출구, 수집 가능 위치 및 시작 위치가 있어야 합니다.
■ 지도에 유효한 경로가 있는지 확인할 필요가 없습니다.
■ 지도는 직사각형이어야 합니다.
■ 지도 규칙을 존중하는 한 모든 종류의 지도를 구문 분석할 수 있어야 합니다.
- 파일에 잘못된 종류의 구성이 있는 경우 프로그램이 올바르게 종료되고 "Error\n"을 반환한 후 선택한 명시적 오류 메시지가 표시되어야 합니다.

## Bonus

- 접촉 시 플레이어의 손실을 초래하는 적이 순찰을 해야합니다.
- 스프라이트 애니매이션이 있어야 합니다.
- 쉘 출력 대신 화면에 이동 횟수가 직접 표시되어야 합니다.
