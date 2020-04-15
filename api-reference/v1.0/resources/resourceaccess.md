---
title: Тип ресурса Ресаурцеакцесс
description: Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ffc1dc7b6a5c76903245f71d0d562a743b37f4d1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368213"
---
# <a name="resourceaccess-resource-type"></a>Тип ресурса Ресаурцеакцесс

Пространство имен: microsoft.graph

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
|id|GUID|Уникальный идентификатор для одного из экземпляров [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md) , предоставляемых приложением ресурсов.|
|type|String|Указывает, ссылается ли свойство **ID** на объект [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md). Возможные значения: "Scope" или "role".|

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
