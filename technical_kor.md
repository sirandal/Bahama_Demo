# Omnione Technical review (v1.0)

1. BlockChain

우리 OmniOne 블록체인은 DPOS+aBFT를 변형한 합의 알고리즘을 사용하고 있으며 속도가 빠른 것이 장점이다. 초당 2000건 이상을 처리하는 합의 속도를 통하여 DID서명 검증, Verifiable Claim 발급처리, 검증 수행등을 실시간에 가깝게 응답해 줄 수 있다. 인증 전용 블록체인 플랫폼 OmniOne은 기존 중앙집중식 인프라 위에 동작하던 인증시장을 블록체인 인프라로 교체함과 동시에 구성원들이 블록체인 기반 서비스를 이용함에 따라 OMN 토큰으로 보상받게 함으로써 인증과 경제발전을 동시에 가져올 수 있다고 기대하고 있다.

블록체인에서 수행되는 기본적인 기능은 DID관리와 또 인증에 대한 처리 등이 주된 것으로 어떤 개인정보도 수집하지 않도록 설계되었다. 또 각종 Verifiable Claim을 발급할수 있는 Issuer를 쉽게 참여 할 수 있게 설계 함으로써 Issuer는 보다 적은 비용으로 인증에 대한 인프라를 제공할 수 있고 또 그 인증을 필요로 하는 Service Provider는 기존에 오프라인 기반에서 제공하던 서비스를 보다 저렵하게 제공할 뿐만 아니라 불가능에 가까웠던 사용자 확인에 대한 시장에서의 요구를 만족시킬수 있게 되었다.



![omniSW](https://github.com/OmniOne-Blockchain/Bahama_Demo/blob/master/img/omniSW.png)


2. DID 를 이용한 자주적 신원 증명

OmniOne은 자주적 디지털 신원(Self-sovereign digital identity) 제공을 목표로 하는 블록체인 기반의 탈중앙 신원 플랫폼 (Decentralized identity Platform)이다.

DID 스팩 (W3C) 을 기반으로 OmniOne 만의 DID method 스팩 (https://github.com/OmniOneID/did_method)을 구현 하였으며 이를 옴니원 블록체인에 저장 함으로써 과거 PKI 환경이 해결하지 못한 공개키 전달 문제를 획기적으로 해결하였다.

OmniOne DID는 ID와 공개키가 포함된 JSON 데이터 형식으로 이루어지며 이러한 내용을 블록체인에 저장하여 DID Entity가 스스로의 신원을 주장할 때 누구의 주장이 진짜인지 쉽게 확인이 가능하게 한다.

블록체인에는 사용자 ID별 DID 문서가 통째로 저장되어 있으며 DID 문서 안에는 DID 스팩에 따라 decentralized ID 및 해당 DID의 공개키 모음이 들어 있다.

블록체인 원장에 저장되어 있는 사용자 DID 문서는  변조및 제거가 불가능하다. 이것이 블록체인과 DID가 결합된 모습이며 DID 기반의 각종 인증이 가능하게 하는 보안적 인프라가 되는 것이다.



3. DID 개인키의 안전한 보관과 FIDO

![img](https://lh3.googleusercontent.com/Hf3xDcxLRFZEGujG4Qlh_tMOcmAHdsafHHScKpdrvtX0icRTFmCC_dbSqEc-PnB_kgO0u2sXFsWChgZPp-akDkZ2cPU09mir9DU-cbWm5xZo_UypeBd6yY11QqEIDouyIQgBGw)

OmniOne은 사용자가 Online Service 또는 Web Service를 이용할 때 Device에 강력한 보안 매커니즘을 제공한다. OmniOne은 기존의DID 스팩이 명확하게 제시하지 못하는 개인키 관리에 대한 부분을 FIDO의 생체 인증에 위임 함으로써 SSI에 보다 강력한 Security로 서비스를 제공할 수 있도록 설계 되었다.

OmniOne은 DID가 만들어 주는 dPKI 위에 FIDO를 접합하여 Security를 강화함으로써 궁극적으로 dFIDO를 구현 해내었다.



4. Verifiable Credential

![credential](https://www.w3.org/TR/verifiable-claims-data-model/diagrams/credential.svg)

출처:https://www.w3.org/TR/verifiable-claims-data-model/

DID를 이용한 Verifiable Credential 은 OmniOne에서 DID기반의 User에게 특정 자격을 부여한 Claim이다. W3C 스팩 (https://www.w3.org/TR/verifiable-claims-data-model/) 을 준수하여 개발 하였으며 여기에 OmniOne만의 증명 별 Level과 Issuer의 가격 정책을 표현하도록 하였다. Verifiable Claim은 User가 기본적으로 소유하고 있는 DID 기반으로 Proof가 만들어져 필요 시에 제출되며 블록체인에서 DID 기반으로 검증 됨으로써 이해 당사자 간에 신뢰관계가 형성된다.

OmniOne Token (OMN)은 Verifiable Claim을 발급 할 수 있는 (User의 데이터를 소유한) Issuer와 이를 확인하여 서비스를 제공하는 Service Provider간의 가치의 교환을 블록체인 기반으로 중계자 없이 가능하게 하였으며 OMN 토큰은 자연스럽게 각 Actor에게 보상으로 돌아가게 된다.

이렇게 DID 기반 Verifiable Credential이 사용됨에 따라 OMN 토큰의 보상이 각 Actor에게 돌아가게 하는것이 우리가 Public에서 설계하고 있는 Ecosystem이며 데모를 통해 어떻게 이 OMN 토큰이 사용되는지 간단하게 보여줄 것이다.


5. 개인정보와 Data Hub

DID 는 개개인에게 개인정보의 주권을 돌려주었다. 과거 개인정보가 한번 기관에 제출되면 사용자의 동의 없이 개인정보는 기관에 의해 점유되고 사용된것과는 달리 DID를 이용하면 개인정보가 사용자의 의도되로만 (목적, 기간) 사용될수 있게 된다.

개인이 점유한 단말에만 개인정보가 있는 경우 개인정보를 수시로 필요로하는 서비스에 적용하기 어려운 문제가 있다. 따라서 자신의 개인정보를 분산 저장소에 안전하게 보관하고 , 해당 정보에 대한 이용처를 개인이 선택할 수 있다 개인정보가 일원화되고, 단말 분실시 개인정보 복구 및 서비스 접근성 용이해진다.

이를 위해 OMN Data Hub를 제공한다. 개인정보는 개인의 의지에 안전하게 Data Hub에 보관 및 유통 되며 언제든제 회수가 가능하다.

![img](https://lh3.googleusercontent.com/68VS5-vNLK4XF-_faQ2sy7y12S9KFTyMJ76cCNC4udUGb5sBWh-CCQcfMkSq3U36pUrHYdGOhxHqQFQP44LTqzPVrPyzV5FbRrjlfvyLKffleNtmWOP4j_uDQgDFxq6WW-aYug)
