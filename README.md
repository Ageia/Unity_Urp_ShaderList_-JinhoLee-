# Unity_URP_ShaderList
  
-FX_SubGraph_MotionVector

![모션_벡터_테스트2](https://user-images.githubusercontent.com/10443544/84388020-d9286e00-ac2e-11ea-8dbe-6c081cf7cb48.gif)

[![Watch the video](https://user-images.githubusercontent.com/10443544/84588153-da8cad00-ae5f-11ea-9810-3db8eebc3e06.png)](https://youtu.be/1efJybmJ870)

  1. 모션 벡터 텍스쳐는 sRGB를 반드시 꺼주세요. (데이터 기반이라 리니어로 처리 해야됩니다)
  2. 모션 벡터 텍스쳐의 G값을 OneMinus 해주세요. (쉐이더 안에 넣을려고 했는데 연산 조금이라도 줄일려고 뺐습니다.)
  3. MotionAmount값은 매우 민감합니다. 0.01~0.025와 같이 낮은 값에서 조절 해주세요.
  4. 5x5타일에서 제대로 재생이 안되는 문제가 있습니다. (유니티 플립북 버그 인거 같은데 원인 못찾았네요.)
  
  
![녹화_2020_11_12_18_59_49_206](https://user-images.githubusercontent.com/10443544/99161796-10003400-2739-11eb-81f2-a67db8fb6544.gif)

1. 그라데이션 서브 그래프를 넣은 뒤 필요한 데이터를 모두 넣고 프로퍼티의 Reference이름을 서브 그래프의 데이터 이름과 일치 시킵니다.
2. 마스터 노드의 ShaderGUI의 이름을 GradientGUI로 입력 해주시면 됩니다.
3. 그라데이션 프로퍼티의 이름은 Color0의 프로퍼티 이름을 그대로 가져옵니다.
