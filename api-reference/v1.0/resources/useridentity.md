---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD это сведения о пользователях, которые инициировали или были затронуты действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 1abc846321e59434053a7a33b3aa8b993a0f9edc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136964"
---
# <a name="useridentity-resource-type"></a>Тип ресурса userIdentity

Пространство имен: microsoft.graph

В контексте журнала аудита Azure AD это сведения о пользователях, которые инициировали или были затронуты действиями аудита.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| displayName | String | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или не всегда в курсе.    |
| id          | String | Уникальный идентификатор удостоверения.  |
| ipAddress   | String| Указывает IP-адрес клиента, используемый пользователем, выполнив действие (только в журнале аудита).|
| userPrincipalName | String  | Атрибут userPrincipalName пользователя. |

>**Примечание.** В некоторых случаях уникальный идентификатор может быть не доступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="json-representation"></a>Представление JSON

Вот представление типа в JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

