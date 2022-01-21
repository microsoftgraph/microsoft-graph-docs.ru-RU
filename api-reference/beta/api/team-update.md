---
title: Обновление объекта команды
description: Обновление свойств указанной команды.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 10603cbd1e5fc2fccefb2c4235cec5d008b04d91
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126825"
---
# <a name="update-team"></a>Обновление объекта команды

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств указанной [группы.](../resources/team.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | TeamSettings.ReadWrite.All, Group.ReadWrite.All **, Directory.ReadWrite.All** |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Application | TeamSettings.ReadWrite.Group *, TeamSettings.ReadWrite.All, Group.ReadWrite.All**, Directory.ReadWrite.All** |

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent). Разрешения, отмеченные **, не используются и не должны использоваться.

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В теле запроса поставляют представление JSON объекта [группы.](../resources/team.md)

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json

{  
 "isMembershipLimitedToOwners": true,
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-team-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->