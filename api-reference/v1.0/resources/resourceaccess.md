---
title: тип ресурса ResourceAccess
description: Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 8986b14e5dba79eaf989fd0a6bf6a4ed479f5aa0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333150"
---
# <a name="resourceaccess-resource-type"></a>тип ресурса ResourceAccess

Пространство имен: microsoft.graph

Объект, используемый для указания области разрешений OAuth 2.0 или роли приложения, которая требуется приложению, через свойство **resourceAccess** типа ресурса [requiredResourceAccess](requiredresourceaccess.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор роли приложения [или](approle.md) [делегированного разрешения](permissionScope.md) , выставленного приложением ресурса. Для делегирования разрешений это должно соответствовать свойству **id** одного из делегированных разрешений в коллекции **oauth2PermissionScopes** доверенного представителя [службы приложения-ресурса](serviceprincipal.md).[](permissionscope.md) Для ролей приложений (разрешений приложений) это должно соответствовать свойству **id** роли [](approle.md) приложения в коллекции **appRoles** основного владельца [службы приложения ресурса](serviceprincipal.md).|
|type|Строка|Указывает, ссылается ли свойство **id** на делегирование разрешения или роль [приложения](approle.md) (разрешение приложения).[](permissionscope.md) Возможные значения: `Scope` (для делегирования разрешений) или `Role` (для ролей приложения).|

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
  "id": "Guid",
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

