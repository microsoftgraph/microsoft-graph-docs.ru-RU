---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD это сведения о пользователях, которые инициировали или были затронуты действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 814b7106bf738711099d6d6e8d5e821b7b638318
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292163"
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
  ]
}
-->

