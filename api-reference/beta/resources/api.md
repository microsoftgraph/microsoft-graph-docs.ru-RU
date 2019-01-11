---
title: Тип ресурса API
description: Задает параметры для приложения Web API.
localization_priority: Normal
ms.openlocfilehash: 50c21c31fec7434514408e1a214c6edf2b838c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845210"
---
# <a name="api-resource-type"></a>Тип ресурса API

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает параметры для приложения Web API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| Указывает версию маркера обслуживаемых доступа для текущего ресурса API. Возможные значения: 1 или 2.  |
|oauth2PermissionScopes|[permissionScope](permissionscope.md) коллекции| Коллекция OAuth 2.0 области разрешений, предоставляемых веб-приложению API (ресурс) на клиентские приложения. Эти области разрешений могут быть предоставлены на клиентские приложения во время подтверждения. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
