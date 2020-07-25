# AccountApi

회원가입및/Profile/포인트 전담 API입니다.

참고: 
- Core JWT : https://jasonwatmore.com/post/2018/08/14/aspnet-core-21-jwt-authentication-tutorial-with-example-api#app-settings-development-json 
- Core JWT : https://jasonwatmore.com/post/2019/10/11/aspnet-core-3-jwt-authentication-tutorial-with-example-api
- JWT : https://tansfil.tistory.com/58?category=255594
- OAuth 2.0 : https://tansfil.tistory.com/60
- Refresh Token : https://fullstackmark.com/post/19/jwt-authentication-flow-with-refresh-tokens-in-aspnet-core-web-api
- Refresh Token : https://medium.com/@kedren.villena/refresh-jwt-token-with-asp-net-core-c-25c2c9ee984b
- Decode  TOken : https://developer.okta.com/blog/2019/06/26/decode-jwt-in-csharp-for-authorization

# RanDev Build

    docker login randev.lunasoft.co.kr:8086 -u lunadev -p lunadev

    docker build -f AccountApi/Dockerfile --force-rm -t randev.lunasoft.co.kr:8086/showa-accountapi-app:dev --label "com.microsoft.created-by=visual-studio" --label "com.microsoft.visual-studio.project-name=accountapi" .

    docker run -e ASPNETCORE_ENVIRONMENT=Development --publish 5005:5000 --name showa-accountapi randev.lunasoft.co.kr:8086/showa-accountapi-app:dev

    http://localhost:5005/swagger/index.html

    docker push randev.lunasoft.co.kr:8086/showa-accountapi-app:dev


"# qwer" 
