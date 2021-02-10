---
title: Тип ресурса conditionalAccessPolicy
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, которые определяют сценарий доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55517d33e7ae933e360118b36b56ad8e8088b50a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153468"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Тип ресурса conditionalAccessPolicy

Пространство имен: microsoft.graph

Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, которые определяют сценарий доступа. Дополнительные сведения см. в [документации по условному доступу.](/azure/active-directory/conditional-access/)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список conditionalAccessPolicies](../api/conditionalaccessroot-list-policies.md) | Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md) | Получите все объекты conditionalAccessPolicies в организации. |
| [Создание conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Создание объекта conditionalAccessPolicy. |
| [Get conditionalAccessPolicy](../api/conditionalaccesspolicy-get.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Чтение свойств и связей объекта conditionalAccessPolicy. |
| [Обновление conditionalAccessPolicy](../api/conditionalaccesspolicy-update.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | Обновление объекта conditionalAccessPolicy. |
| [Удаление conditionalAccessPolicy](../api/conditionalaccesspolicy-delete.md) | Нет | Удаление объекта conditionalAccessPolicy. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|conditions|[conditionalAccessConditionSet](conditionalaccessconditionset.md)| Определяет правила, которые должны быть выполнены, чтобы применить политику. Обязательный элемент. |
|createdDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Readonly. |
|displayName|String| Указывает отображаемое имя объекта conditionalAccessPolicy. |
|grantControls|[conditionalAccessGrantControls](conditionalaccessgrantcontrols.md)| Указывает элементы управления предоставлением, которые должны быть выполнены для прохода политики. |
|id|String| Указывает идентификатор объекта conditionalAccessPolicy. Только для чтения.|
|modifiedDateTime| DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Readonly. |
|sessionControls|[conditionalAccessSessionControls](conditionalaccesssessioncontrols.md)| Указывает элементы управления сеансом, которые применяются после регистрации. |
|состояние|string| Указывает состояние объекта conditionalAccessPolicy. Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`. Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
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