# <a name="authenticate-microsoft-graph-apps-with-the-azure-ad-v20-endpoint"></a>Проверка подлинности в приложениях Microsoft Graph с использованием конечной точки Azure AD версии 2.0

> **Создаете приложения для корпоративных клиентов?** Приложение может не работать, если корпоративный клиент включит функции корпоративной безопасности для мобильных устройств, например <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">условный доступ с устройств</a>.  

> Для поддержки **всех корпоративных клиентов** в **любых корпоративных сценариях** необходимо использовать конечную точку Azure AD и управлять приложениями с помощью [портала управления Azure](https://aka.ms/aadapplist). Дополнительные сведения см. в разделе [Выбор между конечными точками Azure AD и Azure AD версии 2.0](auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).


С помощью конечной точки Azure AD версии 2.0 в можете создавать приложения, которые принимают как рабочие и учебные (Azure Active Directory), так и личные (учетная запись Майкрософт) удостоверения.

Ранее, чтобы обеспечить в приложении поддержку учетных записей Майкрософт и Azure Active Directory, требовалось выполнять интеграцию с двумя отдельными системами. Теперь конечная точка Azure AD версии 2.0 обеспечивает поддержку обоих типов учетных записей с помощью единой интеграции — простого процесса, позволяющего достичь аудитории, насчитывающей миллионы пользователей с личными, рабочими и учебными учетными записями.  

После интеграции приложений с помощью конечной точки Azure AD версии 2.0 они мгновенно получают доступ к конечным точкам Microsoft Graph, доступным для личных и рабочих или учебных учетных записей, например: 

| Данные              | Конечная точка                                       |
|:------------------|:-----------------------------------------------|
| Профиль пользователя      | `https://graph.microsoft.com/v1.0/me`          |
| Почта Outlook      | `https://graph.microsoft.com/v1.0/me/messages` |
| Контакты Outlook  | `https://graph.microsoft.com/v1.0/me/contacts` |
| Календари Outlook | `https://graph.microsoft.com/v1.0/me/events`   |
| OneDrive          | `https://graph.microsoft.com/v1.0/me/drive`    |

 >**Примечание.** Некоторые конечные точки Microsoft Graph, такие как группы и задачи, не применимы к личным учетным записям.  

## <a name="microsoft-graph-authentication-scopes"></a>Области проверки подлинности Microsoft Graph

Конечная точка Azure AD версии 2.0 поддерживает все разрешения, перечисленные в статье [Области разрешений Microsoft Graph](permission_scopes.md). 

Дополнительные сведения об использовании разрешений с конечной точкой Azure AD версии 2.0 и о том, как она отличается от ресурсов в Azure AD, см. в разделе <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#scopes-not-resources" target="_newtab">Области, а не ресурсы</a>.

## <a name="see-it-in-action"></a>Наглядные примеры

[Примеры Connect в репозитории Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) иллюстрируют проверку подлинности пользователей и подключение к Microsoft Graph на множестве платформ.

Кроме того, в разделе [Начало работы](http://developer.microsoft.com/en-us/graph/docs/platform/get-started) указаны статьи, содержащие руководства по созданию этих примеров, в том числе сведения о библиотеках проверки подлинности, используемых на каждой платформе.

## <a name="see-also"></a>См. также

- [Регистрация приложения с помощью конечной точки Azure AD версии 2.0](auth_register_app_v2.md)
- [Проверка подлинности в приложении с помощью Microsoft Graph](auth_overview.md)
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare" target="_newtab">В чем отличия конечной точки версии 2.0?</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/" target="_newtab">Следует ли мне использовать конечную точку версии 2.0?</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/?product=active-directory&term=azure+ad+v2.0" target="_newtab">Документация по конечной точке Azure AD версии 2.0 на сайте Azure.com</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-app-registration/#build-a-quick-start-app" target="_newtab">Краткие руководства по созданию кода для Azure AD версии 2.0 на сайте Azure.com</a>

