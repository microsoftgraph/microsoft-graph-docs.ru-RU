---
title: тип ресурса conditionalAccessPolicy
description: Представляет политику Azure Active Directory доступа. Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1d7e21da89155fa174e4396b4807b2cde4f0b2bf18ae0e2bc19fbfcdf819279f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231875"
---
# <a name="conditionalaccesspolicy-resource-type"></a>тип ресурса conditionalAccessPolicy

Пространство имен: microsoft.graph

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
|conditions|[conditionalAccessConditionSet](conditionalaccessconditionset.md)| Указывает правила, которые необходимо соблюдать для применения политики. Обязательный элемент. |
|createdDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Readonly. |
|displayName|String| Указывает имя отображения объекта conditionalAccessPolicy. |
|grantControls|[conditionalAccessGrantControls](conditionalaccessgrantcontrols.md)| Указывает элементы управления грантами, которые необходимо выполнить для выполнения политики. |
|id|String| Указывает идентификатор объекта conditionalAccessPolicy. Только для чтения.|
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
