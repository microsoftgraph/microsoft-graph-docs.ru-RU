---
title: Тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые активируются соответствующим действием входа.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fe1f31555c2ea809d50faf87a1041f527a5ddc74
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695337"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>Тип ресурса appliedConditionalAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые активируются соответствующим действием входа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|authenticationStrength|[authenticationStrength](authenticationstrength.md)| Надежность пользовательской проверки подлинности, применяемая в политике условного доступа.|
|conditionsNotNot|conditionalAccessConditions|Относится к условиям политики условного доступа, которые не удовлетворяются. Возможные значения: `none`, , `application`, `users`, `devicePlatform`, `location`, `signInRisk``clientType`, `userRisk`, `time`, `deviceState`,`ipAddressSeenByAzureAD``client`,,`unknownFutureValue``ipAddressSeenByResourceProvider`,,.`servicePrincipals``servicePrincipalRisk` Обратите внимание, что необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса для получения следующих значений в этом развиваемом [перечислении](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipals`,`servicePrincipalRisk`.|
|conditionsИмя|conditionalAccessConditions|Ссылается на условия политики условного доступа, которые выполняются. Возможные значения: `none`, , `application`, `users`, `devicePlatform`, `location`, `signInRisk``clientType`, `userRisk`, `time`, `deviceState`,`ipAddressSeenByAzureAD``client`,,`unknownFutureValue``ipAddressSeenByResourceProvider`,,.`servicePrincipals``servicePrincipalRisk` Обратите внимание, что необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса для получения следующих значений в этом развиваемом [перечислении](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipals`,`servicePrincipalRisk`.|
|displayName|String|Имя политики условного доступа.|
|enforcedGrantControls|Коллекция строк|Относится к элементам управления предоставлением, применяемым политикой условного доступа (например, "Требовать многофакторную проверку подлинности").|
|enforcedSessionControls|Коллекция String|Относится к элементам управления сеансом, применяемым политикой условного доступа (например, "Требовать элементы управления, принудительно применяемые приложением").|
|excludeRulesА|[Коллекция conditionalAccessRule Темы](conditionalaccessrulesatisfied.md)|Список пар "ключ-значение", содержащих каждое соответствующее условие исключения в политике условного доступа. Пример: `[{"devicePlatform" : "DevicePlatform"}]` означает, что политика не применена, так как условие DevicePlatform совпадает.|
|id|String|Идентификатор политики условного доступа.|
|includeRulesИмя|[Коллекция conditionalAccessRule Темы](conditionalaccessrulesatisfied.md)|Список пар "ключ-значение", содержащих каждое соответствующее условие, включается в политику условного доступа. Пример. `[{ "application" : "AllApps"}, {"users": "Group"}]`Это означает, что условие приложения совпадает, так как включены allApps, а условие "Пользователи" совпадает, так как пользователь был частью включенного правила группы.|
|result|appliedConditionalAccessPolicyResult| Указывает результат активируемой политики ЦС. Возможные значения: `success`, , `failure`, `notApplied` (Политика не применяется, так как условия политики не были выполнены),`notEnabled` (Это связано с политикой в отключенном состоянии), `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, , `reportOnlyNotApplied``reportOnlyInterrupted`. Обратите внимание, что необходимо использовать `Prefer: include-unknown-enum-members` заголовок запроса для получения следующих значений в этом развиваемом перечислении[:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`reportOnlySuccess` , `reportOnlyFailure`, , . `reportOnlyNotApplied``reportOnlyInterrupted`|
|sessionControlsNot|Коллекция строк|Относится к элементам управления сеансом, которые не были выполнены действием входа. (Пример: `Application enforced Restrictions`).|




## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "@odata.type": "#microsoft.graph.appliedConditionalAccessPolicy",
  "id": "String (identifier)",
  "authenticationStrength": {"@odata.type": "microsoft.graph.authenticationStrength"},
  "displayName": "String",
  "enforcedGrantControls": [
    "String"
  ],
  "enforcedSessionControls": [
    "String"
  ],
  "conditionsSatisfied": "String",
  "conditionsNotSatisfied": "String",
  "includeRulesSatisfied": [
    {
      "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
    }
  ],
  "excludeRulesSatisfied": [
    {
      "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
    }
  ],
  "result": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
