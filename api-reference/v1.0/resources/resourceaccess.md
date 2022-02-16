---
title: тип ресурса ResourceAccess
description: Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 82cbf3f8823b53d45f89013d97892fc4ba5c751b
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854468"
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

