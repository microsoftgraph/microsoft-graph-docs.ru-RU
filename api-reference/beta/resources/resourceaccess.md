---
title: тип ресурса ResourceAccess
description: Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: cd971de84841068ffa8a7a4af7b3258c5f45003f
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451418"
---
# <a name="resourceaccess-resource-type"></a>тип ресурса ResourceAccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, используемый для указания области разрешений OAuth 2.0 или роли приложения, которая требуется приложению, через свойство **resourceAccess** типа ресурса [requiredResourceAccess.](requiredresourceaccess.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор для одного из [экземпляров oauth2PermissionScopes](permissionscope.md) или экземпляров [appRole,](approle.md) которые предоставляет приложение ресурса.|
|type|String|Указывает, ссылается ли свойство **id** на [oauth2PermissionScopes](permissionscope.md) или [appRole.](approle.md) Возможные значения: `Scope` (для областей разрешений OAuth 2.0) или `Role` (для ролей приложений).|

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
  "id": "GUID",
  "type": "String"
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


