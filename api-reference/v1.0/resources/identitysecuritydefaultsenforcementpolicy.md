---
title: тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику Azure Active Directory безопасности по умолчанию. По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.
ms.localizationpriority: medium
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 07dcd2efc5fa7f83c10993293cd23c740003ef0b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032379"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>тип ресурса identitySecurityDefaultsEnforcementPolicy

Пространство имен: microsoft.graph

Представляет политику Azure Active Directory безопасности по [умолчанию.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.

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
|displayName|String|Отображение имени для этой политики. Только для чтения.|
|id|Строка|Идентификатор для этой политики. Только для чтения.|
|isEnabled|Boolean|Если установлено `true` значение , Azure Active Directory по умолчанию безопасности включен для клиента.|

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
