---
title: тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику безопасности по умолчанию Azure Active Directory. По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 249396b0c2bfc4b39ca21c198958adc3d0b9e228
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945647"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>тип ресурса identitySecurityDefaultsEnforcementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику безопасности по умолчанию Azure Active [Directory.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.

Наследует [от policyBase](../resources/policybase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/identitysecuritydefaultsenforcementpolicy-get.md); | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Ознакомьтесь с свойствами **объекта identitySecurityDefaultsEnforcementPolicy.** |
| [Обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Обновление **объекта identitySecurityDefaultsEnforcementPolicy.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка|Описание этой политики. Только для чтения.|
|displayName|Строка|Отображение имени для этой политики. Только для чтения.|
|id|Строка|Идентификатор для этой политики. Только для чтения.|
|isEnabled|Boolean|Если установлено значение, по умолчанию `true` безопасность Azure Active Directory включена для клиента.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
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
