---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 304d5a27714d7e6e02183b372814c8cb16c4e0b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446795"
---
# <a name="useridentity-resource-type"></a>Тип ресурса userIdentity

Пространство имен: microsoft.graph

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
