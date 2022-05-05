---
title: Получение groupSetting
description: Получение свойств определенного объекта параметра группы.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 885408ec1e6cfad786d7c07f422f8e975955c3dc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209382"
---
# <a name="get-groupsetting"></a>Получение groupSetting

Пространство имен: microsoft.graph

Получение свойств определенного объекта параметра группы. Параметр может быть параметром уровня клиента или группы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="list-tenant-wide-settings"></a>Вывод списка параметров на уровне клиента

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Directory.Read.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Directory.Read.All, Directory.ReadWrite.All |

### <a name="list-group-specific-settings"></a>Перечисление параметров для конкретной группы

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Group.Read.All, Group.ReadWrite.All         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Group.Read.All, Group.ReadWrite.All         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

Получение параметра на уровне клиента.

```http
GET /groupSettings/{groupSettingId}
```

<!-- { "blockType": "ignored" } -->

Получение параметра для конкретной группы.

```http
GET /groups/{groupId}/settings/{groupSettingId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметр `$select` [запроса OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [groupSetting](../resources/groupsetting.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-a-group-setting-for-a-specific-group"></a>Пример 1. Получение параметра группы для определенной группы

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/05aa6a98-956a-45c0-b13b-88076a23f2cd/settings/a06fa228-3042-4662-bd09-33e298da1afe
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
    "id": "a06fa228-3042-4662-bd09-33e298da1afe",
    "displayName": "Group.Unified.Guest",
    "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
    "values": [
        {
            "name": "AllowToAddGuests",
            "value": "false"
        }
    ]
}
```

### <a name="example-2-get-the-group-settings-for-all-microsoft-365-groups"></a>Пример 2. Получение параметров группы для всех Microsoft 365 групп

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_groupsettings_tenantwide"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-tenantwide-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-tenantwide-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-tenantwide-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-tenantwide-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-tenantwide-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-tenantwide-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-tenantwide-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-tenantwide-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-tenantwide-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-tenantwide-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
    "id": "84af2ca5-c274-41bf-86e4-6e374ec4def6",
    "displayName": "Group.Unified",
    "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "values": [
        {
            "name": "EnableMIPLabels",
            "value": "true"
        },
        {
            "name": "CustomBlockedWordsList",
            "value": ""
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "value": "true"
        },
        {
            "name": "ClassificationDescriptions",
            "value": ""
        },
        {
            "name": "DefaultClassification",
            "value": ""
        },
        {
            "name": "PrefixSuffixNamingRequirement",
            "value": "[Contoso-][GroupName]"
        },
        {
            "name": "AllowGuestsToBeGroupOwner",
            "value": "false"
        },
        {
            "name": "AllowGuestsToAccessGroups",
            "value": "true"
        },
        {
            "name": "GuestUsageGuidelinesUrl",
            "value": "https://privacy.contoso.com/privacystatement"
        },
        {
            "name": "GroupCreationAllowedGroupId",
            "value": ""
        },
        {
            "name": "AllowToAddGuests",
            "value": "true"
        },
        {
            "name": "UsageGuidelinesUrl",
            "value": ""
        },
        {
            "name": "ClassificationList",
            "value": ""
        },
        {
            "name": "EnableGroupCreation",
            "value": "true"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
