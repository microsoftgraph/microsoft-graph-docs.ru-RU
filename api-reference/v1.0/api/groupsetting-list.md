---
title: Параметры группы списка
description: Извлечение списка объектов группового настройки.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: af51f4fd21e1d17316b08b0ea99f87d315431e57
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027726"
---
# <a name="list-group-settings"></a>Параметры группы списка

Пространство имен: microsoft.graph

Извлечение списка объектов группового настройки.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

Список параметров клиента или группы.

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

>**Примечание.** $filter не поддерживается.

## <a name="request-headers"></a>Заголовки запросов
| Имя | Описание |
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [groupSetting](../resources/groupsetting.md) в тексте ответа.
## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groupsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик

Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings",
  "value": [
    {
      "id": "f0b2d6f5-097d-4177-91af-a24e530b53cc",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

