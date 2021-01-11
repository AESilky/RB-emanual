Instruction Packet으로 장치를 식별하기 위한 고유 번호입니다.  
0~252 (0xFC) 까지 사용 가능하며, 254(0xFE)는 브로드캐스트(Broadcast) ID로 특수하게 사용됩니다.  
브로드캐스트 ID(254, 0xFE)로 Instruction Packet을 전송하면 모든 장치에 명령을 내릴 수 있습니다.

**참고** : 연결된 장치의 ID가 중복되지 않도록 주의해야 합니다. 또한 ID(7)는 EEPROM 영역에 존재하기 때문에 [Torque Enable(64)] 의 값이 ’0’ 일 때만 변경할 수 있습니다.
{: .notice}

**참고** : Instruction packet 의 ID가 Broadcast ID(0xFE) 인 경우는 이 값에 상관 없이 Status Packet이 반환되지 않습니다. 더 자세한 설명은 [Protocol 1.0] 와 [Protocol 2.0]의 `Status Packet` 항목을 참조하심시오.
{: .notice}
