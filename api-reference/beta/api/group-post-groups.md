---
title: Создание группы
description: Создание группы Office 365 или группы безопасности.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: c91c43c0156aa4edda9eef71232001fdede38887
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536199"
---
# <a name="create-group"></a>Создание группы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса. Можно создать одну из следующих групп:

* Группа Office 365 (единая группа)
* Группа безопасности

Эта операция по умолчанию возвращает только подмножество свойств для каждой группы. Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).

Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`. См. [пример](group-get.md#request-2).

>**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

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
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы. 

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| displayName | string | Имя, которое следует отобразить в адресной книге для группы. Обязательный. |
| mailEnabled | boolean | Установите значение **true** для групп, поддерживающих почту. Обязательно. |
| mailNickname | string | Почтовый псевдоним для группы. Обязательный. |
| securityEnabled | boolean | Значение **true** для защищенных групп, включая группы Office 365. Обязательно. |
| owners | Коллекция [directoryObject](../resources/directoryobject.md) | Это свойство представляет владельцев группы на момент создания. Необязательный параметр. |
| members | Коллекция [directoryObject](../resources/directoryobject.md) | Это свойство представляет участников группы на момент создания. Необязательный параметр. |

> **Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.

Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.

>**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.  Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.  

При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).

### <a name="grouptypes-options"></a>Параметры groupTypes

Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.

| Тип группы | Назначенное участие | Динамическое участие |
|:--------------|:------------------------|:---------------|
| Office 365 (как единая группа)| `["Unified"]` | `["Unified","DynamicMembership"]`
| Динамическая группа | `[]` (_null_) | `["DynamicMembership"]`|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика. Отклик включает в себя только свойства по умолчанию для группы.

## <a name="examples"></a>Примеры

### <a name="example-1-create-an-office-365-group"></a>Пример 1. Создание группы Office 365

В следующем примере создается группа Office 365.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. В результате реального вызова возвращаются все свойства по умолчанию.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a>Пример 2. Создание группы Office 365 с владельцем и участниками

В следующем примере создается группа Office 365 с указанным владельцем и участниками.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a>Отклик 

Ниже представлен пример успешного отклика. Он включает только свойства по умолчанию. Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. В результате реального вызова возвращаются все свойства по умолчанию.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>Дополнительные ресурсы

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
