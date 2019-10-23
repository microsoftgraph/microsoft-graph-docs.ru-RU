---
title: Тип ресурса Кондитионалакцессполици
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8187e98d1ddc5a096dea469bea22681fd5df78e7
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637762"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Тип ресурса Кондитионалакцессполици

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа. Дополнительные сведения см. в [документации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список КондитионалакцессполиЦиес](../api/conditionalaccessroot-list-policies.md) | Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md) | Получение всех объектов КондитионалакцессполиЦиес в Организации. |
| [Создание Кондитионалакцессполици](../api/conditionalaccessroot-post-policies.md) | [кондитионалакцессполици](conditionalaccesspolicy.md) | Создание нового объекта Кондитионалакцессполици. |
| [Получение Кондитионалакцессполици](../api/conditionalaccesspolicy-get.md) | [кондитионалакцессполици](conditionalaccesspolicy.md) | Чтение свойств и связей объекта Кондитионалакцессполици. |
| [Обновление Кондитионалакцессполици](../api/conditionalaccesspolicy-update.md) | [кондитионалакцессполици](conditionalaccesspolicy.md) | Обновление объекта Кондитионалакцессполици. |
| [Удаление Кондитионалакцессполици](../api/conditionalaccesspolicy-delete.md) | Нет | Удаление объекта Кондитионалакцессполици. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|conditions|[кондитионалакцесскондитионсет](conditionalaccessconditionset.md)| Задает правила, которые должны выполняться для применения политики. Обязательный элемент. |
|createdDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Статического. |
|description|String| Не используется. |
|displayName|Строка| Задает отображаемое имя для объекта Кондитионалакцессполици. |
|грантконтролс|[кондитионалакцессгрантконтролс](conditionalaccessgrantcontrols.md)| Указывает элементы управления предоставлением, которые должны быть выполнены для передачи политики. |
|id|String| Задает идентификатор объекта Кондитионалакцессполици. Только для чтения.|
|modifiedDateTime| DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Статического. |
|сессионконтролс|[кондитионалакцесссессионконтролс](conditionalaccesssessioncontrols.md)| Задает элементы управления сеансом, которые применяются после входа. |
|состояние|string| Задает состояние объекта Кондитионалакцессполици. Возможные значения: `enabled`, `disabled`. Обязательный элемент. |

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
  "baseType": "",
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
