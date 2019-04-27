---
title: Тип ресурса API
description: Задает параметры для приложения веб-API.
localization_priority: Normal
ms.openlocfilehash: f26a568d05c85059e914b355d971755f19627cac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348422"
---
# <a name="api-resource-type"></a>Тип ресурса API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает параметры для приложения веб-API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|Рекуестедакцесстокенверсион|Int32| Указывает принятую версию маркера доступа для текущего ресурса API. Возможные значения: 1 или 2.  |
|oauth2PermissionScopes|Коллекция [permissionScope](permissionscope.md)| Коллекция областей разрешений OAuth 2,0, предоставляемых приложением веб-API (ресурсом) для клиентских приложений. Эти области разрешений могут быть назначены клиентским приложениям во время согласия пользователя. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
