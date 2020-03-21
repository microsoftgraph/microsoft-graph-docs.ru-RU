---
title: Тип ресурса Идентитисекуритидефаултсенфорцементполици
description: Представляет политику безопасности по умолчанию для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3cb792b59281c05cc915649bf3b689714438bd93
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896047"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>Тип ресурса Идентитисекуритидефаултсенфорцементполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику [безопасности по умолчанию](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.

Наследуется от [основы](../resources/policybase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/identitysecuritydefaultsenforcementpolicy-get.md); | [идентитисекуритидефаултсенфорцементполици](identitysecuritydefaultsenforcementpolicy.md) | Чтение свойств объекта **идентитисекуритидефаултсенфорцементполици** . |
| [обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md). | [идентитисекуритидефаултсенфорцементполици](identitysecuritydefaultsenforcementpolicy.md) | Обновление объекта **идентитисекуритидефаултсенфорцементполици** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание для этой политики. Только для чтения.|
|displayName|Строка|Отображаемое имя для этой политики. Только для чтения.|
|id|String|Идентификатор для этой политики. Только для чтения.|
|isEnabled|Boolean|Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySecurityDefaultsEnforcementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
