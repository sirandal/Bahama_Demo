# Bahama Demo Overview



#### 데모 개요

OmniOne은 서로 신뢰할 수 있는 세상을 만드는 것을 목적으로 한다.

블록체인과 DID를 기반으로 한 신뢰 인프라가 구축되어 있다는 가정하면  Issuer는 자신들이 원하는 Verifiable Claim을 OmniOne을 통해 사용자에게 발급한다.

사용자는 사회 전반에 구축된 OmniOne 자격 증명을 사용할수록 OMN 토큰으로 OmniOne 플래폼을 통해 보상받게 되며 이렇게 쌓인 사용자의 OMN 토큰이 직접 지불 수단으로 사용되어 측정할 수 없을 만큼의 사회 경제적 선진화가 이루어지게 된다.

우리는 이 데모를 통하여 사용자가 Korean인 Eliot이 바하마를 여행하는데 있어 얻는 편의와 그동안 상상할 수 없었던 경제적 순환을 보여주고자 한다.

바하마에 입국하는 순간부터 본국으로 돌아갈 때까지 방문객 Eliot이 겪는 경제적 혜택을 이 데모를 통해 느껴보도록 한다.



#### 시나리오 1 : 온라인 몰

바하마에 방문하는 여행객 Eliot은 바하마 입국 심사대에서 여권을 제출한다. 방문자의 여권정보는 바하마의 기관에 디지털 정보로 저장된다. 그리고 이 정보는 사용자가 바하마 방문자용 디지털 신분증 발급받기 위한 기반 데이터베이스로 활용 되게 된다.

바하마에 도착한 Eliot은 바하마 관광 안내에 따라 OmniOne 앱을 설치하고 해당 앱을 통해 방문자용 디지털 신분증을 발급 받는다. 그리고 해당 발급에 대한 보상으로 10000 OMN을 지급 받게 된다.

![vc](https://github.com/OmniOne-Blockchain/Bahama_Demo/blob/master/img/vc.png)



관광 안내서에는 방문객이 이용할 수 있는 온라인 몰의 링크를 확인할 수 있다.

온라인 쇼핑몰에  접속한 Eliot은 별도의 회원가입 없이 OmniOne 앱을 통해 부여받은 방문자용 디지털 신분증을 통해 쇼핑몰에 Sign In 할수 있다. (Verifiable Claim)

쇼핑몰에는 바하마에서 제공하는 관광 상품으로 이루어져 있고 가격도 OMN 단위로 표기되어 있다. 물품을 선택하고 결제를 누르면 OmniOne 앱을 통해 결재하고 최초 발급에 대한 포상으로 받은 10000 OMN 중 일부를 사용하여 결제가 완료 된다. 앱에서 나의 토큰을 확인하면 상품 가격이 차감되어 있음을 확인할 수 있다.

시나리오 1에서는 사용자의 Verifiable Claim으로 KYC가 필요할 수 있는 쇼핑몰에 자동으로 회원 가입되는 부분, 또 DID를 이용한 서명을 통해 블록체인에 저장된 나의 토큰을 사용하는 예제를 설명하였다.



#### 시나리오 2 : 오프라인 매장

시나리오 2에서는 오프라인에서 사용자의 방문객 자격을 확인하는 시나리오를 설명하고자 한다. 매장에 붙어 있는 QR 코드를 사용자가 OmniOne 앱으로 촬영한다. QR코드 내에는 가게 주인의 DID 정보와 방문객이 해당 매장에서 이용하려고 하는 서비스에 가격이 표시되어 있다.

방문객은 앱에서 상대방에 대한 정보 및 액수를 확인하고 생체 인증을 통해 전자서명한다. 나의 앱에서 토큰이 차감되었음을 확인한다.

매장에서는 매장이 관리하는 페이지를 통해 사용자가 결제한  토큰이 추가 되었음을 확인한다.

![Bahamas_QR_1](https://github.com/OmniOne-Blockchain/Bahama_Demo/blob/master/img/Bahamas_QR_1.png)

#### Demo Infomation

App download URL: 

Online Service Page URL: http://iw.whitehat.co.kr/omnionedemo

Offline Service Page URL: 

Admin Page URL : http://iw.whitehat.co.kr/omnionedemo/console/login (admin/12345)

동영상 :

