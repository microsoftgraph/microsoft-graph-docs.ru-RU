# <a name="delete-open-extension"></a>Удаление открытого расширения

Удаление открытого расширения (объекта [openTypeExtension](../resources/openTypeExtension.md)) из указанного экземпляра ресурса. 

## <a name="prerequisites"></a>Необходимые условия

Для выполнения этого API требуется одно из указанных **разрешений** (в зависимости от ресурса, из которого удаляется расширение):

|**Поддерживаемый ресурс**|**Разрешение**|**Поддерживаемый ресурс**|**Разрешение** |
|:-----|:-----|:-----|:-----|
| [device](../resources/device.md) | _Device.ReadWrite.All_ | [event](../resources/event.md) | _Calendars.ReadWrite_ |
| [group](../resources/group.md) | _Group.ReadWrite.All_ | [group event](../resources/event.md) | _Group.ReadWrite.All_ |
| [group post](../resources/post.md) | _Group.ReadWrite.All_ | [message](../resources/message.md) | _Mail.ReadWrite_ |
| [organization](../resources/organization.md) | _Directory.AccessAsUser.All_ | [contact](../resources/contact.md) (личный контакт) | _Contacts.ReadWrite_ |
| [user](../resources/user.md) | _Directory.AccessAsUser.All_ | | |

 
## <a name="http-request"></a>HTTP-запрос
В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

>**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.

## <a name="parameters"></a>Параметры
|**Параметр**|**Тип**|**Описание**|
|:-----|:-----|:-----|
|_Параметры URL-адреса_|
|id|string|Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.|
|extensionId|string|Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.|


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Значение |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

Во втором примере показано, как удалить расширение в событии указанной группы.

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a>Отклик
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->