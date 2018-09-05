# <a name="create-group"></a>Создание группы
Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:

* Группа Office 365 (единая группа)
* Динамическая группа
* Группа безопасности

> **Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Авторизация  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В таблице ниже представлены свойства ресурса [group](../resources/group.md) для указания при создании группы. 

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| displayName | string | Имя для отображения в адресной книге для группы. Обязательное. |
| mailEnabled | boolean | Устанавливает значение **true** для групп с поддержкой почты. Установите значение **true** при создании группы Office 365. Установите значение **false** при создании динамической группы или группы безопасности. Обязательное. |
| mailNickname | string | Почтовый псевдоним для группы. Обязательное. |
| securityEnabled | boolean | Значение **true** для групп с поддержкой безопасности. Установите значение **true** при создании динамической группы или группы безопасности. Установите значение **false**при создании группы Office 365. Обязательное. |
| владельцы | коллекция строк | Это свойство представляет владельцев группы во время создания. Необязательный параметр. |
| члены | коллекция строк | Это свойство представляет членов группы во время создания. Необязательный параметр. |


При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.

### <a name="grouptypes-options"></a>Параметры groupTypes

| Тип группы | Свойство **groupTypes** |
|:--------------|:------------------------|
| Office 365 (как единая группа)| "Unified" |
| Динамическая группа | "DynamicMembership" |
| Система безопасности | Не следует устанавливать. |


>**Примечание.** При создании группы Office 365 программными средствами без контекста пользователя и указания владельцев будет создана анонимная группа.  Это может привести к тому, что связанный сайт SharePoint Online не будет создаваться автоматически, пока не будут вручную предприняты дальнейшие действия.  

При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика.

## <a name="example"></a>Пример
#### <a name="request-1"></a>Запрос 1
В первом примере запроса создается группа Office 365.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a>Отклик 1
Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>Запрос 2
Во втором примере запроса создается группа Office 365 с указанными владельцами.
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a>Отклик 2
Ниже приведен пример успешного отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
