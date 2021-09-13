---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD это представляет сведения пользователей, которые инициировали или пострадали от действий аудита.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 621574365bc8c14508eb87dc55df60f1fd9a3f08
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136301"
---
# <a name="useridentity-resource-type"></a>Тип ресурса userIdentity

Пространство имен: microsoft.graph

В контексте журнала аудита Azure AD это представляет сведения пользователей, которые инициировали или пострадали от действий аудита.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| displayName | Строка | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или в курсе.    |
| id          | String | Уникальный идентификатор удостоверения.  |
| ipAddress   | String| Указывает IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).|
| userPrincipalName | String  | Атрибут userPrincipalName пользователя. |

>**Примечание:** В некоторых случаях уникальный идентификатор может оказаться недоступным. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="json-representation"></a>Представление JSON

Вот представление JSON этого типа.

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

