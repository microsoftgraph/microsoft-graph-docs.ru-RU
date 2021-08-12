---
title: тип ресурса ResourceAccess
description: Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0d5c8a60b1080b1e605dde754d8007cf15b36b129d276a6b2d9f87421ba9ef25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243317"
---
# <a name="resourceaccess-resource-type"></a>тип ресурса ResourceAccess

Пространство имен: microsoft.graph

Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению. Свойство **resourceAccess** типа [requiredResourceAccess](requiredresourceaccess.md) — это коллекция **ResourceAccess.**

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор для одного из [экземпляров oauth2PermissionScopes](permissionscope.md) или экземпляров [appRole,](approle.md) которые предоставляет приложение ресурса.|
|type|String|Указывает, ссылается ли свойство **id** на [oauth2PermissionScopes](permissionscope.md) или [appRole.](approle.md) Возможные значения: `Scope` или `Role`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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

