---
title: Тип ресурса Идентитисекуритидефаултсенфорцементполици
description: Представляет политику безопасности по умолчанию для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13c7fd24c7f7d96149821a8a4e506e32ae681c78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086699"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>Тип ресурса Идентитисекуритидефаултсенфорцементполици

Пространство имен: microsoft.graph

Представляет политику [безопасности по умолчанию](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.

Наследуется от [основы](../resources/policybase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [идентитисекуритидефаултсенфорцементполици](identitysecuritydefaultsenforcementpolicy.md) | Чтение свойств объекта **идентитисекуритидефаултсенфорцементполици** . |
| [Обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [идентитисекуритидефаултсенфорцементполици](identitysecuritydefaultsenforcementpolicy.md) | Обновление объекта **идентитисекуритидефаултсенфорцементполици** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка|Описание для этой политики. Только для чтения.|
|displayName|Строка|Отображаемое имя для этой политики. Только для чтения.|
|id|Строка|Идентификатор для этой политики. Только для чтения.|
|isEnabled|Boolean|Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.|

## <a name="relationships"></a>Связи

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

