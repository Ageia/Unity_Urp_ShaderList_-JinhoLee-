# Unity_URP_ShaderList
  
-FX_SubGraph_MotionVector

![모션_벡터_테스트2](https://user-images.githubusercontent.com/10443544/84388020-d9286e00-ac2e-11ea-8dbe-6c081cf7cb48.gif)

[![Watch the video](https://user-images.githubusercontent.com/10443544/84396238-3de8c600-ac39-11ea-8def-cb062cbcd659.png)](https://youtu.be/1efJybmJ870)

  1. 모션 벡터 텍스쳐는 sRGB를 반드시 꺼주세요. (데이터 기반이라 리니어로 처리 해야됩니다)
  2. 모션 벡터 텍스의 G값을 OneMinus 해주세요. (쉐이더 안에 넣을려고 했는데 연산 조금이라도 줄일려고 뺐습니다.)
  3. MotionAmount값은 매우 민감합니다. 0.01~0.025와 같이 낮은 값에서 조절 해주세요.
  4. 5x5타일에서 제대로 재생이 안되는 문제가 있습니다. (유니티 플립북 버그 인거 같은데 원인 못찾았네요.)
