---
title: Тип ресурса governanceRoleSetting
description: " правила и т. д."
ms.openlocfilehash: 64245b2d6f0aa9e0ea3ffda4a5eaebfb9fd205df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079099"
---
# <a name="governancerolesetting-resource-type"></a>Тип ресурса governanceRoleSetting

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет набор конфигураций на каждое определение роли, которое должно использоваться для вычисления при создании или измененные назначения ролей. К примеру параметры роли могут содержать правила «назначения Максимальная длительность», «Многофакторной проверкой Подлинности требуется на активации» правила и т.д.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [governanceRoleSetting](../resources/governancerolesetting.md) коллекции|Список коллекцию параметров роли для ресурса.|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Чтение свойства и связи параметров ролей.|
|[Update](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Обновите объект параметров роли. |

## <a name="properties"></a>Свойства
|Свойство               |Тип                                      |Описание|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |Идентификатор roleSetting.|
|resourceId           |String                                  |Обязательно. Идентификатор ресурса, с которым связана параметров ролей.|
|roleDefinitionId     |Строка                                  |Обязательно. Идентификатор определения роли, с которым связана параметров ролей.|
|isDefault            |Логический                                 |Только для чтения. Укажите, является ли roleSetting roleSetting по умолчанию|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметров ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|lastUpdatedBy        |String                                  |Только для чтения. Отображаемое имя администратора, который последним обновил roleSetting.|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.|
|adminMemberSettings  |[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.|
|userEligibleSettings |[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли. Параметр не поддерживается в данный момент.|
|userMemberSettings   |[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются при попытке активировать его назначения ролей.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанные ресурсов для этого параметра роли.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, которое применяется при использовании этого параметра роли. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
