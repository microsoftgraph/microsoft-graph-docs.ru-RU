# <a name="app-authentication-with-microsoft-graph"></a>Проверка подлинности в приложении с помощью Microsoft Graph

Чтобы получать доступ к данным учетных записей Майкрософт, приложение должно предоставлять пользователю возможности пройти проверку подлинности и разрешить приложению выполнять действия от его имени.

Microsoft Graph поддерживает двух поставщиков проверки подлинности:

- Для проверки подлинности пользователей с личными учетными записями Майкрософт, например _live.com_ и _outlook.com_, используется [конечная точка Azure Active Directory (Azure AD) версии 2.0](converged_auth.md).
- Для проверки подлинности пользователей с корпоративными (то есть, рабочими или учебными) учетными записями используется [Azure AD](app_authorization.md).


> **Создаете приложения для корпоративных клиентов?** Приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>.  

> Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist).

![Стек приложения Microsoft Graph с проверкой подлинности в виде слоя между приложением и различными ресурсами Microsoft Graph.](./images/MSGraph_DevStack_v2Auth.png)

## <a name="deciding-between-the-azure-ad-and-azure-ad-v20-endpoints"></a>Выбор между конечными точками Azure AD и Azure AD версии 2.0

В приведенной ниже таблице представлена сводка основных функций, поддерживаемых конечными точками Azure AD и Azure AD версии 2.0, а также приводятся ссылки на дополнительные сведения. Относительная важность этих функций — и, следовательно, выбранный поставщик проверки подлинности для приложения — в основном зависит от следующих показателей:

- Тип учетных записей (корпоративные или клиентские), которые должны поддерживать приложения
- Тип создаваемого приложения
- Необходимый поток проверки подлинности 

<table style="width:100%">
  <tr>
    <th></th>
    <th>Конечная точка Azure AD</th> 
    <th>Конечная точка Azure AD версии 2.0</th>
   </tr>
  <tr>
    <td>Поддерживаемые типы предоставления</td>
    <td style="vertical-align: text-top;"><p>Код авторизации</p><p>Неявный поток</p><p>Учетные данные клиента</p><p>Учетные данные владельца ресурса</p></td> 
    <td style="vertical-align: text-top;"><p>Код авторизации</p><p>Неявный поток</p><p>Учетные данные клиента</p></td>
   </tr>
  <tr>
    <td>Поддерживаемые типы приложений</td>
    <td style="vertical-align: text-top;"><p>Веб-приложения</p><p>Веб-API</p><p>Мобильные и собственные приложения</p><p>Одностраничное приложение (SPA)</p><p>Автономные веб-API</p><p>Управляющие программы и серверные приложения</p><p><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/" target="_newtab">дополнительные сведения</a></p></td> 
    <td style="vertical-align: text-top;"><p>Веб-приложения</p><p>Веб-API</p><p>Мобильные и собственные приложения</p><p>Одностраничное приложение (SPA)</p><p>Управляющие программы и серверные приложения</p><p><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/" target="_newtab">дополнительные сведения</a></td>
   </tr>
  <tr>
    <td>Политики условного доступа с устройств</td>
     <td><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">Поддерживаются</a></td> 
    <td>В настоящее время не поддерживается</td>
   </tr>
  <tr>
    <td>Поддержка OAuth 2.0 и OpenID Connect</td>
    <td>Нет</td> 
    <td>Да</td>
  </tr>
  <tr>
    <td>Permissions</td>
    <td>Статические: указываются во время регистрации </td> 
    <td><a href ="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#scopes-not-resources" target="_newtab">Динамические:</a> запрос во время выполнения приложения; включает добавочное согласие</td>
  </tr>
  <tr>
    <td>Типы учетных записей</td>
    <td> <p>рабочая или учебная</p></td> 
    <td><p>рабочая или учебная</p><p>личная</p> </td>
  </tr>
  <tr>
    <td>Идентификатор приложения </td>
    <td>Отдельный идентификатор приложения для каждой платформы</td> 
    <td><a href ="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#one-app-id-for-all-platforms" target="_newtab">Один идентификатор приложения для нескольких платформ</a></td>
  </tr>
  <tr>
    <td>Портал регистрации </td>
    <td><a href ="https://manage.windowsazure.com/" target="_newtab">Портал управления Microsoft Azure</a></td> 
    <td><a href ="https://apps.dev.microsoft.com" target="_newtab">Портал регистрации приложений (Майкрософт)</a></td>
  </tr>
  <tr>
    <td>Клиентские библиотеки </td>
    <td>Пакеты SDK проверки подлинности Active Directory (ADAL) для большинства платформ разработки</td> 
    <td><p><a href="https://www.nuget.org/packages/Microsoft.Identity.Client" target="_newtab">Предварительная версия библиотеки аутентификации (Майкрософт)</a></p><p><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/#restrictions-on-libraries-amp-sdks" target="_newtab">Библиотеки OAuth 2.0 с открытым кодом (список)</a></p> </td>
  </tr>
  <tr>
    <td>Другие функции </td>
    <td><p>Утверждения о группах для пользователей Azure AD</p><p>Роли приложений и утверждения о ролях</p></td> 
    <td></td>
  </tr>
</table> 

Кроме того, существуют различия между областями разрешений, которые требуются двум поставщикам проверки подлинности, а также между утверждениями, возвращаемыми в разных маркерах. Дополнительные сведения см. в разделах [Хорошо известные области](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#well-known-scopes) и [Утверждения маркера](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#token-claims) статьи [В чем отличия конечной точки версии 2.0?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/).

Кроме того, конечная точка Azure AD версии 2.0 находится в активной разработке — планируется добавить новые функции и поддерживаемые сценарии. Текущий список ограничений для конечной точки Azure AD версии 2.0 см. в статье [Следует ли мне использовать конечную точку версии 2.0?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/).

## <a name="registering-your-app-for-authentication"></a>Регистрация приложения для проверки подлинности 

Если вы решили, какой поставщик проверки подлинности соответствует требованиям вашего приложения, вам потребуется зарегистрировать приложение на портале этого поставщика. При регистрации приложения создается его удостоверение, связанное с поставщиком проверки подлинности, которое приложение может указывать при отправке запросов на проверку подлинности от имени пользователя.

- Чтобы зарегистрировать приложение с помощью Azure AD, используйте [портал Azure](https://portal.azure.com/).

    <!--For Azure AD, you'll also need to associate your Office 365 account with Azure AD subscription in order to manage your apps.-->

- Чтобы [зарегистрировать приложение с помощью конечной точки Azure AD версии 2.0](auth_register_app_v2.md), используйте [портал регистрации приложений (Майкрософт)](https://apps.dev.microsoft.com).


## <a name="resources-for-implementing-authentication-in-your-microsoft-graph-app"></a>Ресурсы для реализации проверки подлинности в приложении Microsoft Graph 

Когда вы зарегистрируете приложение на соответствующем портале проверки подлинности и получите сведения о регистрации приложения (идентификатор и секрет приложения, а также, при необходимости, URI перенаправления), необходимые для создания удостоверения, вы будете готовы реализовать проверку подлинности в приложении. 

Опять же, это зависит от типа создаваемого приложения, платформы разработки, выбранного потока проверки подлинности, а также от конкретных требований к проверке подлинности в этом приложении. 

### <a name="connect-samples-by-authentication-provider-and-platform"></a>Приложения Connect для разных поставщиков проверки подлинности и платформ

Ниже представлены приложения Connect для разных поставщиков проверки подлинности и платформ, а также указано, что они используют для подключения к Microsoft Graph: REST или клиентскую библиотеку Microsoft Graph.

<table>
  <tr>
    <th>Платформа</th>
    <th>Конечная точка Azure AD</th> 
    <th>Конечная точка Azure AD версии 2.0</th>
  </tr>
  <tr>
    <td>Android</td>
    <td>Пример с использованием 
        <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST</a> или <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">пакета SDK</a>
    </td> 
    <td>
        <a href="https://github.com/microsoftgraph/android-java-connect-sample">Пример с использованием пакета SDK</a>
    </td> 
  </tr>
  <tr>
    <td>ASP.NET</td>
    <td>
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">Пример с использованием REST</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">Пример с использованием пакета SDK</a>
    </td> 
  </tr>
  <tr>
    <td>iOS (Obj-C)</td>
    <td>
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">Пример с использованием REST</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">Пример с использованием пакета SDK</a>
    </td> 
  </tr>
  <tr>
    <td>iOS (Swift)</td>
    <td>
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">Пример с использованием REST</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">Пример с использованием пакета SDK</a>
    </td> 
  </tr>
  <tr>
    <td>Node.js</td>
    <td>
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">Пример с использованием REST</a>
    </td> 
  </tr>
  <tr>
    <td>PHP</td>
    <td>
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample">Пример с использованием REST</a>
    </td> 
  </tr>
  <tr>
    <td>Python</td>
    <td>
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">Пример с использованием REST</a>
    </td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td>Ruby</td>
    <td>
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">Пример с использованием REST</a>
    </td> 
  </tr>
  <tr>
    <td>UWP</td>
    <td>
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a>
    </td>     
    <td>Пример с использованием 
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST</a> или <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">пакета SDK</a>
    </td> 
  </tr>
  <tr>
    <td>Xamarin</td>
    <td>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">Пример с использованием пакета SDK</a>
    </td> 
  </tr>
</table>

Широкий ассортимент проектов, подключающихся к Microsoft Graph с использованием различных технологий, вы найдете в [репозитории Microsoft Graph](https://github.com/microsoftgraph) на сайте GitHub. 

### <a name="get-started"></a>Начало работы  

В разделе [Начало работы](http://developer.microsoft.com/en-us/graph/docs/platform/get-started) представлены подробные статьи, посвященные созданию перечисленных в таблице приложений с использованием конечной точки Azure AD версии 2.0, а также рассматриваются библиотеки проверки подлинности, используемые на каждой из платформ. 

## <a name="see-also"></a>См. также

- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#basics-of-authentication-in-azure-ad" target="_newtab">Сценарии проверки подлинности для Azure AD</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/?product=active-directory&term=v2.0+endpoint" target="_newtab">Документация по конечной точке Azure AD версии 2.0 на сайте Azure.com</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-app-registration/#build-a-quick-start-app" target="_newtab">Краткие руководства по созданию кода для Azure AD версии 2.0 на сайте Azure.com</a>
