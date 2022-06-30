---
title: Вывод группы
description: Получение свойств и связей объекта group.
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6fccabf60e9f625a638f61d0e52053aec31ce28d
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555928"
---
# <a name="get-group"></a>Вывод группы 

Пространство имен: microsoft.graph

Получение свойств и связей объекта group.

Это действие по умолчанию возвращает только часть всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties). Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`. Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.

> **Примечание.** При запросе могут происходить задержки репликации для групп, которые были недавно созданы, обновлены или удалены.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Делегированное (рабочая или учебная учетная запись)     | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                                                                                         |
| Для приложений                            | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |

> **Примечание.** В зависимости от функций группы, к которым вы пытаетесь получить доступ, разрешения могут быть ограничены. Дополнительные сведения см. в разделе [Группы](/graph/known-issues#groups) статьи [Известные проблемы с Microsoft Graph](/graph/known-issues).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.

Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).

### <a name="retrieve-extensions-and-associated-data"></a>Извлечение расширений и связанных данных

| Тип расширения       | Комментарии                                                                       |
|----------------------|--------------------------------------------------------------------------------|
| Расширения схемы    | Возвращается только с помощью `$select`.                                                  |
| Открытые расширения      | Возврат через операцию [Получение открытого расширения](opentypeextension-get.md). |
| Расширения каталога | Возвращается по умолчанию.                                                           |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика. Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.

## <a name="example"></a>Пример

### <a name="example-1-return-all-default-properties"></a>Пример 1. Возвращение всех свойств по умолчанию

Возвращение всех свойств по умолчанию.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса GET.

<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. Он содержит только свойства по умолчанию.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове возвращаются все свойства, используемые по умолчанию.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/b320ee12-b1cd-4cca-b648-a437be61c5cd/Microsoft.DirectoryServices.Group",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-13T10:07:01Z",
    "creationOptions": [],
    "description": "Self help community for library",
    "displayName": "Library Assist",
    "expirationDateTime": "2022-01-11T10:07:01Z",
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": null,
    "mail": "library@contoso.com",
    "mailEnabled": true,
    "mailNickname": "library",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "EU",
    "preferredLanguage": null,
    "proxyAddresses": [
        "SPO:SPO_0dbffe23-f6fb-4478-adcd-880daf88bb12@SPO_84841066-274d-4ec0-a5c1-276be684bdd3",
        "SMTP:library@contoso.com"
    ],
    "renewedDateTime": "2021-09-13T10:07:01Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "securityIdentifier": "S-1-12-1-1306860066-1319449225-59104187-458188010",
    "theme": null,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-return-additional-properties-by-using-select"></a>Пример 2. Возвращение дополнительных свойств с помощью параметра $select

Возвращение дополнительных свойств с помощью параметра `$select`.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса GET.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-group-non-default-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-group-non-default-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-group-non-default-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/get-group-non-default-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
