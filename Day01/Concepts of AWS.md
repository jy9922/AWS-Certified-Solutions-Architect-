# 1. AWS Cloud

### AWS Cloud

- 2002년 아마존에서 시작되었다.
- AWS는 복잡하고 확장 가능한 애플리케이션을 만들 수 있다.
- 다양한 산업 분야에서 적용할 수 있다.

### AWS Global Infrastructure

- AWS에는 리전, 가용영역(AZ), 데이터 센터가 있다.
- AWS Edge Location / Points of Presence(전송 지점)

### Regions

- 리전은 전 세계에 걸쳐 있다.
- **데이터 센터의 집합**이다.
- AWS 서비스를 사용할 때 대부분의 서비스들은 특정 리전에 연결되어 국한된다.
    - 한 리전에서 어떤 서비스를 사용하다가 다른 리전에 서비스를 사용하게 되면 서비스를 처음 사용하는 것과 같게된다.
- 어느 리전을 선택하는 것이 좋을까? 고려사항
    - **법률 준수** - 정부는 애플리케이션을 배포할 때 대상 국각 내에 데이터가 보관되기를 원한다.
        
        [http://m.ddaily.co.kr/m/m_article/?no=259905](http://m.ddaily.co.kr/m/m_article/?no=259905)
        
    - **지연 시간** - 대부분의 사용자가 미국에 있는 경우라면, 애플리케이션 또한 사용자와 가까이 있는 것이 좋다.
    - **서비스의 유무** : 모든 리전에 모든 서비스가 있는 것은 아니기에 확인이 필요하다.
    - **요금** - 리전마다 요금이 다르다.

### Availability Zones

- 리전 내에 존재한다.
- 대부분은 3개이다. (min2 ~ max 6)
- 각각의 가용 영역은 여분의 전원, 네트워킹, 통신 기능을 갖춘 하나 또는 두 개의 개별적인 데이터 센터로 이루어져 있다.
- 각각 가용 영역은 재난 발생에 대비해 서로 분리되어 있다.
- 데이터 센터와 가용 영역들은 높은 대역폭의 초저지연 네트워킹으로 서로 연결되어 있어 리전을 형성한다.

### AWS Points of Presence(Edge Locations)

- 42개국 84개의 도시에 200개가 넘는 전송 지점을 가지고 있다.
- 이런 점으로 최소 지연 시간으로 최종 사용자에게 컨텐츠를 전달하는데 매우 유용하다.

### AWS Console

- AWS의 글로벌 서비스
    - IAM, Route 53, CloudFront, WAF
- 특정 리전에 국한되는 서비스
    - EC2(IaaS)
    - Elastic Beanstalk(PaaS)
    - Lambda(FaaS)
    - Rekognition(SaaS)