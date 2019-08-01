---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e72f5338f7281188b7023aed342dd34ee57595e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033504"
---
# <a name="useridentity-resource-type"></a>Тип ресурса userIdentity

В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| displayName | Строка | Отображаемое имя удостоверения. Обратите внимание, что эта возможность не всегда доступна или не актуальна.    |
| id          | String | Уникальный идентификатор удостоверения.  |
| ipAddress   | String| IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).|
| userPrincipalName | String  | Атрибут userPrincipalName пользователя. |

>**Примечание:** В некоторых случаях уникальный идентификатор может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление типа в формате JSON.

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
