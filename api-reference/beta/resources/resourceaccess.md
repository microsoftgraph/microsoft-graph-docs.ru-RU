---
title: Тип ресурса Ресаурцеакцесс
description: Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением. Свойство **ресаурцеакцесс** типа рекуиредресаурцеакцесс является коллекцией **ресаурцеакцесс**.
localization_priority: Normal
ms.openlocfilehash: bb77a12a207e274b27263029d96f4ef260cfe5cb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343635"
---
# <a name="resourceaccess-resource-type"></a>Тип ресурса Ресаурцеакцесс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением. Свойство **ресаурцеакцесс** типа [рекуиредресаурцеакцесс](requiredresourceaccess.md) является коллекцией **ресаурцеакцесс**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор для одного из экземпляров [oAuth2Permission](oauth2permission.md) или [аппроле](approle.md) , предоставляемых приложением ресурсов.|
|type|String|Указывает, ссылается ли свойство **ID** на объект [oAuth2Permission](oauth2permission.md) или [аппроле](approle.md). Возможные значения: "Scope" или "role".|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
