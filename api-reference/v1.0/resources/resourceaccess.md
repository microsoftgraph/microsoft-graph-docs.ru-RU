---
title: тип ресурса ResourceAccess
description: Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 18b1c5b3f42b3f7203363a95b94ed1cf036e7fed
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347999"
---
# <a name="resourceaccess-resource-type"></a>тип ресурса ResourceAccess

Пространство имен: microsoft.graph

Объект, используемый для указания области разрешений OAuth 2.0 или роли приложения, которая требуется приложению, через свойство **resourceAccess** типа ресурса [requiredResourceAccess](requiredresourceaccess.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор роли приложения [или](approle.md) [делегированного разрешения](permissionScope.md) , выставленного приложением ресурса. Для делегирования разрешений это должно соответствовать свойству **id** одного из делегированных разрешений в коллекции **oauth2PermissionScopes** доверенного представителя [службы приложения-ресурса](serviceprincipal.md).[](permissionscope.md) Для ролей приложений (разрешений приложений) это должно соответствовать свойству **id** роли [](approle.md) приложения в коллекции **appRoles** основного владельца [службы приложения ресурса](serviceprincipal.md).|
|type|String|Указывает, ссылается ли свойство **id** на делегирование разрешения или роль [приложения](approle.md) (разрешение приложения).[](permissionscope.md) Возможные значения: `Scope` (для делегирования разрешений) или `Role` (для ролей приложения).|

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

