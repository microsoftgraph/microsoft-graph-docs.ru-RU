---
title: Тип ресурса API
description: Задает параметры для приложения веб-API.
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535693"
---
# <a name="api-resource-type"></a>Тип ресурса API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает параметры для приложения веб-API.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|Рекуестедакцесстокенверсион|Int32| Указывает принятую версию маркера доступа для текущего ресурса API. Возможные значения: 1 или 2.  |
|oauth2PermissionScopes|Коллекция [permissionScope](permissionscope.md)| Коллекция областей разрешений OAuth 2,0, предоставляемых приложением веб-API (ресурсом) для клиентских приложений. Эти области разрешений могут быть назначены клиентским приложениям во время согласия пользователя. |

## <a name="json-representation"></a>Представление в формате JSON
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
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/api.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
