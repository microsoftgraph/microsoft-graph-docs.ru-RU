---
title: Тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику по умолчанию для безопасности Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно заранее задав параметры безопасности, которые защищают от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dea4d94dfc8de8310410498fdf8d83c2a5e8f68
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154931"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a>Тип ресурса identitySecurityDefaultsEnforcementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику по умолчанию для [безопасности](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) Azure Active Directory. Значения по умолчанию для системы безопасности содержат предварительно заранее настраиваемую настройку параметров безопасности, которые защищают от распространенных атак.

Наследуется [от policyBase.](../resources/policybase.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Чтение свойств объекта **identitySecurityDefaultsEnforcementPolicy.** |
| [Обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md) | Обновление объекта **identitySecurityDefaultsEnforcementPolicy.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание этой политики. Только для чтения.|
|displayName|String|Отображаемого имени для этой политики. Только для чтения.|
|id|String|Идентификатор этой политики. Только для чтения.|
|isEnabled|Boolean|Если установлено значение true, для клиента включены значения по умолчанию для системы безопасности Azure Active Directory.|

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