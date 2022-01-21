---
title: тип ресурса conditionalAccessPolicy
description: Представляет политику Azure Active Directory доступа. Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5aa585b12b75a88452dc3dbde7c24d08b60cbcd4
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161678"
---
# <a name="conditionalaccesspolicy-resource-type"></a>тип ресурса conditionalAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику Azure Active Directory доступа. Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа. Дополнительные сведения см. в [документации условного доступа.](/azure/active-directory/conditional-access/)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список conditionalAccessPolicies](../api/conditionalaccessroot-list-policies.md) | Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md) | Получите все объекты conditionalAccessPolicies в организации. |
| [Создание conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Создайте новый объект conditionalAccessPolicy. |
| [Get conditionalAccessPolicy](../api/conditionalaccesspolicy-get.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Чтение свойств и связей объекта conditionalAccessPolicy. |
| [Обновление conditionalAccessPolicy](../api/conditionalaccesspolicy-update.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Обновление объекта conditionalAccessPolicy. |
| [Удаление conditionalAccessPolicy](../api/conditionalaccesspolicy-delete.md) | Нет | Удаление объекта conditionalAccessPolicy. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|conditions|[conditionalAccessConditionSet](conditionalaccessconditionset.md)| Указывает правила, которые необходимо соблюдать для применения политики. Обязательный. |
|createdDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Readonly. |
|description|Строка| Не используется. |
|displayName|Строка| Указывает имя отображения объекта conditionalAccessPolicy. |
|grantControls|[conditionalAccessGrantControls](conditionalaccessgrantcontrols.md)| Указывает элементы управления грантами, которые необходимо выполнить для выполнения политики. |
|id|Строка| Указывает идентификатор объекта conditionalAccessPolicy. Только для чтения.|
|modifiedDateTime| DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Readonly. |
|sessionControls|[conditionalAccessSessionControls](conditionalaccesssessioncontrols.md)| Указывает элементы управления сеансами, которые применяются после регистрации. |
|state|conditionalAccessPolicyState| Указывает состояние объекта conditionalAccessPolicy. Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`. Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "baseType":"microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "grantControls": {"@odata.type": "microsoft.graph.conditionalAccessGrantControls"},
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)",
  "sessionControls": {"@odata.type": "microsoft.graph.conditionalAccessSessionControls"},
  "state": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
