---
title: Тип ресурса Аппроле
description: Представляет роль приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 913531740211a698e00f1a8c62d177d79e6602a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050166"
---
# <a name="approle-resource-type"></a>Тип ресурса Аппроле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль приложения, которая может быть запрошена клиентским приложением (и предоставлена ей), или с помощью которой можно назначить приложение пользователям или группам в указанной роли. 

Свойство **appRoles** сущностей [Application](application.md) и [servicePrincipal](serviceprincipal.md) является коллекцией **аппроле**. 

С помощью [аппролеассигнментс](approleassignment.md)роли приложений могут быть назначены пользователям, группам или субъектам служб других приложений.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|алловедмембертипес|Коллекция String|Указывает, может ли эта роль приложения назначаться пользователям и группам (с помощью параметра `["User"]` ), другим приложениям (по значению `["Application"]` или обоим `["User", "Application"]` ). Роли приложений, поддерживающие назначение субъектов служб других приложений, также называются [разрешениями приложений](/graph/auth/auth-concepts#microsoft-graph-permissions).|
|description|String|Описание роли приложения. Он отображается при назначении роли приложения и, если роль приложения работает как разрешение приложения, во время предоставления согласия.|
|displayName|Строка|Отображаемое имя разрешения, которое отображается при назначении роли приложения и согласия пользователя.|
|id|GUID|Уникальный идентификатор роли в семействе **appRoles** . При создании новой роли приложения необходимо указать новый идентификатор GUID. |
|isEnabled|Boolean|При создании или обновлении роли приложения должно быть задано **значение true** (значение по умолчанию). Чтобы удалить роль, необходимо сначала задать значение **false**.  В этот момент эта роль может быть удалена в последующих вызовах.|
|основания|Строка| Указывает, определена ли роль приложения для объекта [Application](application.md) или объекта [servicePrincipal](serviceprincipal.md) . _Не_ следует включать в запросы POST или patch. Только для чтения. |
|value|String|Указывает значение, которое будет включено в `roles` утверждения маркеров идентификаторов и маркеров доступа, которые проходят проверку подлинности назначенного пользователя или участника службы. Длина не должна превышать 120 символов. Допустимые знаки `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , а также символы в диапазонах `0-9` `A-Z` и `a-z` . Любой другой символ, в том числе символ пробела, не допускается.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


