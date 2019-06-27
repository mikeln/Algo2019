## 대회소개 
------------------------
2013년에 한 부서에서 작은 게임으로 시작했던 알고리즘 경진대회가 이제는 전사 행사를 넘어, 올해는 해외 법인과 자회사 임직원들도 참여하는 커다란 행사가 되었습니다.

이번 알고리즘 경진대회는 차량 운행 시뮬레이터(Microsoft Airsim)를 활용한 자동차 레이스로 진행되며, 룰 기반 주행 과 자율 주행 2개의 부문으로 진행합니다.

룰 주행 부문은 차량의 각 상태에 대응하는 알고리즘을 직접 작성함으로써 차량을 주행시키는 것이고, 자율주행 부문은 주어진 모델을 적절한 보상 함수로 학습시켜서 학습된 모델 에이전트로 차량을 주행시키는 방법 입니다.

룰 주행 부문은 2대의 차량이 대전을 하여 승자를 가리는 방식이며, 친선 리그, 예선(리그) 및 본선(토너먼트)으로 진행됩니다. 자율주행 부문은 트랙 별 싱글 플레이로 기록을 측정하고, ranking 을 매기는 방식으로 진행합니다. 본선에서는 제출된 모델이 여러 트랙을 주행하도록 하여 기록의 종합점수를 가지고 등수를 부여할 예정입니다.



### 룰 기반 대회 상세 안내



예선 리그전은 전체팀을 8개조로 나눠 편성하고, 각 조의 상위 4개팀이 주행기록에 따라 32강 토너먼트에 진출합니다.

온라인 예선과 오프라인 본선을 통해 최종우승자를 가립니다.



### ■ 온라인 예선 (32개팀 선정)

리그 조 내에서 대전을 하여 승패에 따라 점수가 부여되고 순위가 결정되며 상위 4개팀이 32강 진출에 진출합니다. 경기의 승패는 두 팀이 동일 출발지점에서 2바퀴 Lap을 완주한 시간을 기준으로 결정합니다. 두 팀 다 완주하지 못하는 경우, 무승부가 되며, 동점 상황에서 순위 우열을 가릴 때에는 주행거리가 더 긴 쪽이 우선하는 것으로 합니다. 그리고, BOT 사전 점검 오류가 있는 경우, 실격처리하고 해당 조의 차 순위 팀이 32강 진출하는 것으로 합니다.

예선 조는 회사/사업부 단위 참가현황에 맞추어 편성하며 다음의 규칙으로 합니다.

- 조편성은 대회에 참가한 인원에 대한 사업부 별 균형을 고려하여 편성합니다. 대략 8개 조로 구성될 예정입니다.(조별 팀구성/팀수는 참가 현황에 따라 변경 가능)
- 소수 인원이 참가한 사업부는 타사업부와 혼합 편성 될 수 있습니다.


### ■ 오프라인 본선 (16강 이상팀 시상)

32강부터는 토너먼트 대진방식으로 최종 우승자를 선정합니다. 패자는 탈락하고, 승자는 다음 라운드에 진출하여, 최후에 남는 두 팀의 승자가 우승자가 됩니다. 두 팀이 모두 실격할 경우, 주행거리가 더 긴 쪽이 승리하는 것으로 합니다. 두 팀의 출발 위치는 예선 혹은 바로 이전 경기의 성적이 더 우수한 팀이 안쪽이나 앞쪽 지점에서 출발하는 것으로 합니다. 상금이나 부상은 16강 이상 팀부터 주어지며, 16강 이상 팀은 시상을 위해 현장참여가 필요합니다.

### 대진 구성 방식

- 조별 상위 팀은 다른 조의 하위 팀과 대진하도록 구성합니다. (예: A조 1위는 B조 4위, B조 2위는 A조 3위와 대결)





### 자율주행 대회 상세 안내



### ■ 온라인 예선 (트랙 별 주행)

룰 기반과 달리 대전 형태로 진행이 되지 않기 때문에 주행 기록으로 등수를 부여합니다. 트랙을 지정하고 모델을 제출하면, 서버에서 주행을 실행하여 기록을 측정하고 대회 홈페이지 랭킹 페이지에 보여질 예정입니다.

트랙은 순차적으로 오픈 할 예정이고, 본선이 시작되기 전까지 각 트랙 별로 계속해서 모델을 제출하여 기록을 갱신할 수 있습니다. 제출 마감시점까지 트랙 별로 최고 기록을 갱신한 팀에게 상품을 지급할 예정입니다.



### ■ 온라인 본선 (여러 트랙 주행)

본선은 1개 트랙에서만 최적화된 모델이 아닌, 여러 트랙에서 두루두루 잘 주행하도록 훈련된 모델 생성을 목표로 합니다. 본선 진행 시점에 지정된 2개 혹은 3개의 트랙에서 주행한 종합 점수를 가지고 최종 우승자를 가리게 됩니다.



### 대회 실격 처리 기준



### ■ 대회 규칙 (실격 처리)

- 정해진 트랙(도로)에서 이탈 후 지속적으로 복귀하지 않는 경우, 지름길이나 지도 오류 활용시 실격 처리

- 경주 시작 후, 일정시간 (10 min) 이내 완주하지 못하는 경우. 주행을 완료할 수 없는 상태에 도달한 경우도 포함합니다. (차량 전복, 장애물로 인한 주행 불가 등)

- 주행 BOT이 일정시간 (100 millisecond) 이내에 주행 제어를 하지 않는 경우, 기능 오류가 발생하여 정지한 경우

- 주행 트랙의 체크포인트를 비정상적인 방법으로 통과하여 주행하는 경우

- 상대방 차량의 방해 행위나 상대방 차량의 동작오류로 인해 나의 차량 운행이 불가능하게 되는 경우에는 상대방 차량을 실격 처리합니다. 단, 정상적인 앞지르기 방해 등은 해당하지 않으며 상대 차량이 운행불가 상태가 되지 않는 범위 내에서 추돌 및 부딪힘은 허용 합니다.

- 시뮬레이터 조작이나 정하지 않은 주행 환경 설정 변경으로 인한 부정행위 (정해진 주행환경 설정과 기본 제공 API 이외의 개발 방법 적용 시 반드시 대회운영TF에 사전 확인바랍니다.)

- 경기 이후에라도 사후 검토(주행 영상 및 소스코드 확인)를 통해 부정행위가 발견될 경우, 성적은 취소처리 됩니다.



### ■ 그외 규칙

- 예선 트랙/본선 트랙은 대회운영 TF에서 지정합니다.

- 대회 운영 방식은 사정에 따라 변경될 수 있으며, 변경 전 충분히 사전 공지를 할 예정입니다.

<br><br>
---------------
<br><br>

## Introduction  
------------------------
Algorithm Contest started in a department is now became a big event for employees from subsidiaries and overseas subsidiaries this year.

This event is conducted as a car race using vehicle simulator(Microsoft Airsim) and it's divided into two categories: rule-based driving and autonomous driving

In the rule-based driving, the vehicle get actions directly from the algorithm code corresponding to each state of the vehicle, and for the autonomous driving part, a model trained with proper reward function drives the vehicle.


### The detailed information about the rule based driving



The Qualification consists of eight groups, and the top four teams of each group advance to the 32nd tournament according to their result.

The final winners will be selected through online qualification and offline finals.



### On-line Qualification (32 teams selected)

The teams will play in the league and scores will be awarded according to the race result. The top four teams will advance to the 32nd Division. The win or loss is decided by the lap time of the race that the two team completed the two laps, starting from the same starting point. If both team fails to finish, they will be withdrawn and if they are ranked in the tie, the team who raced longer distance will have the priority. And if there is an error in the BOT on the inpection, the team will be disqualified.

We organize the group according to the company / division unit.

- The league group is organized considering the divisional balance of the participants. It is planned to be composed of approximately 8 teams (composition of group / number of teams can be changed depending on participation status)
- Business divisions with a small number of employees can be grouped with other divisions.


### Off-line Main Event (Top 16 teams will be awarded)

From the 32nd, the tournament match begins. The winner advances to the next round. If both teams fail to finish, the team who raced longer distance will win. Regarding starting point, inside position will be given to the team who gets better result from the previous match. Awards and prizes will be awarded to top 16 teams, they must participate in the tournament and awards ceremony.



### How to organize the match

- The teams who ranked high in the group have match with the teams who ranked low in the pother group.(ex: 1st place team in group A will have match with 4th place team in group B, 2nd place team in gruop 2 wil have match with 3rd place team in group A)






### The detailed information about the autonomous driving




### ■ Online Qualification (collects records by each track)

Unlike the rule based driving, it's not competition between users. Instead, we measure the lap time of each team and show rankings on the leader board. If you submit your model by selecting the track, server will run, measure the lap time and the result will be shown on the homepage automatically.

The rest of the track will be opened one by one and the racing records can be submitted until the main event begins. After the deadline, the teams who has the best record will be awarded.




### ■ Online Main event (collects records across multiple tracks)

For the main event, the goal for the paticipants is to create model which is well trained to race not just one specific track but across multiple tracks. The final winner will be decided by overall score running 2 or 3 tracks selected during the main event period.




### Disqualification Standards



### ■ Contest rule (Disqualification)

- If you do not return to the track after departing from the designated track and take advantage of shortcuts or map errors, you will be disqualified.

- If you can not finish within 10 mins after the start of the race, you will be disqualified.

- If the BOT loose the control within 100 mSec or a functional error occurs, you will be disqualified.

- If you pass the checkpoint of the track in an abnormal way, you will be disqualified

- If you make the other team's vehicle impossible to operate or drive, you will be disqualified.However, normal frontal obstruction is allowed and collision and bump are allowed if you do not cause the opponent vehicle's failure or overturning

- Any illegal acts caused by cheating on simulator or environment setting change will be disqualified. (If you want to use other Apis and development method not defined your own (not built-in API), Please be sure to ask the Contest TF in advance).

- After the game, if any cheating is found through a post review (We will check the video and source code), the result will be canceled.



### ■ Other rules

- The tracks for qualification/Main eventis will be selected by the contest TF

- The operating rule of the competition can be changed according to circumstances and will be announced prior to change.
