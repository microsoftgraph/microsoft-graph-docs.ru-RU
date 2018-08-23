# <a name="use-the-onenote-rest-api"></a>Использование REST API для OneNote

Microsoft Graph позволяет вашему приложению получать авторизованный доступ к записным книжкам OneNote, разделам и страницам в личной учетной записи или учетной записи организации. С [соответствующими или делегированными разрешениями приложения](../../../concepts/permissions_reference.md#notes-permissions)ваше приложение может получать доступ к данным OneNote пользователя, выполнившего вход в систему, или любого пользователя в клиенте.

## <a name="root-url"></a>Корневой URL-адрес
Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
Сегмент `version` URL-адреса представляет собой версию Microsoft Graph, которую вы хотите использовать:

- `v1.0` предназначено для стабильного производственного кода.
- `beta` |||UNTRANSLATED_CONTENT_START|||is to try out a feature that's in development.|||UNTRANSLATED_CONTENT_END||| Возможности и функции в конечной точке бета-версии могут изменяться. Мы не рекомендуем использовать её в рабочем коде.

В качестве места расположения могут быть записные книжки пользователя в Office 365 или объекте-получателе OneDrive, групповые записные книжки, или размещенные на сайте SharePoint в Office 365 групповые записные книжки. 

![Стек разработки API-интерфейса OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Записные книжки пользователя
Чтобы получить доступ к персональным записным книжкам объекта-получателя OneDrive или OneDrive для бизнеса, воспользуйтесь одним из следующих URL-адресов:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` |||UNTRANSLATED_CONTENT_START|||is for OneNote content that the current user can access (owned and shared).|||UNTRANSLATED_CONTENT_END|||
- `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. Используйте API[пользователей](users.md).
> **Примечание.** Вы можете получить идентификаторы пользователя, отправив запрос GET на `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Групповые записные книжки
 Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>Записные книжки на сайте SharePoint

Чтобы получить доступ к записным книжкам на узле группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

