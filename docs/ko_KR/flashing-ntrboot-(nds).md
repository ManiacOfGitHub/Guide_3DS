# ntrboot 플래싱 (NDS)

## 중요

진행하기 앞서서, [ntrboot](ntrboot) 에 대한 모든 정보를 숙지해주세요.

이 방법은 DS 플래시카트를 실행할 수 있는 DS 혹은 DS Lite가 필요합니다. 이 방법은 플래시카드를 NDS에 삽입해 ntrboot flasher `.nds` 를 실행하는 방법입니다.

::: danger

아주 드문 경우지만 설치를 시도한 플래시카드가 짝퉁일 경우 설치 과정 중 카트리지가 **벽돌**이 되고 이후 카트리지를 사용할 수 없게되는 경우가 있습니다. 그러하기 때문에 매우 적은 확율이지만 정품 플래시카트만 지원 됩니다. 복재품 카드를 주문할 가능성을 줄이기 위하여, [NDS Card](https://www.nds-card.com/)같이 신뢰할 수 있는 사이트를 이용하여 구매 하시길 바랍니다.

:::

## 준비물

- ntrboot를 설치할 수 있는 플래시카트
- 두 개의 콘솔들
    - **소스 NDS/NDSL**: 플래시카트와 호환되는 닌텐도 DS 또는 DS Lite
    - **타겟 3DS** CFW를 설치할 3DS
- v1.3 버전의 [boot9strap-ntr](https://github.com/SciresM/boot9strap/releases/download/1.3/boot9strap-1.3-ntr.zip) (직접 다운로드)
- 최신 버전의 [ntrboot_flasher_nds](https://github.com/jason0597/ntrboot_flasher_nds/releases/latest) (`ntrboot_flasher_nds.nds`)

## 진행 방법

### 섹션 I - 준비 작업

1. **소스 NDS / NDSL**를 종료해 주세요
2. DS 플래시카트의 SD 카드를 컴퓨터에 삽입해 주세요
3. 플래시카트 SD 카드의 루트에 `ntrboot` 폴더를 만들어 주세요
4. `boot9strap_ntr.firm`과 `boot9strap_ntr.firm.sha`을 boot9strap-ntr `.zip` 에서 플래시카트 SD 카드의 `/ntrboot/` 폴더로 복사해 주세요
5. 플래시카트의 SD 카드에 `ntrboot_flasher_nds.nds`를 복사해 주세요
6. 플래시카트의 SD 카드를 다시 플래시카트에 삽입해 주세요
7. **소스 NDS / NDSL**에 ntrboot와 호환 가능한 DS/DSi 플래시카트를 삽입해 주세요

### 섹션 II - ntrboot 플래싱

1. **소스 NDS / NDSL**에서 플래시카트를 이용해 `ntrboot_flahser_nds.nds`를 실행해 주세요
2. (A)를 눌러 진행해 주세요
3. (위) 버튼과 (아래) 버튼을 눌러 삽입되 있는 플래시카트를 선택해 주세요
4. (A)를 눌러 진행해 주세요
5. "Dump flash"를 선택하여 플래시카트의 메모리를 백업해 주세요
6. 화면에 보이는 버튼 콤보를 눌러 확인해 주세요
7. (A)를 눌러 진행해 주세요
8. (위) 버튼과 (아래) 버튼을 눌러 삽입되 있는 플래시카트를 선택해 주세요
9. (A)를 눌러 진행해 주세요
10. "Inject FIRM"을 선택해 boot9strap를 플래시카트로 설치해 주세요
11. 화면에 보이는 버튼 콤보를 눌러 확인해 주세요
12. (A)를 눌러 진행해 주세요
13. **소스 NDS / NDSL**를 종료해 주세요
14. **소스 NDS / NDSL**에서 플래시카트를 제거해 주세요

___

::: tip

[boot9strap 설치 (ntrboot)](installing-boot9strap-\(ntrboot\))로 계속합니다

:::
