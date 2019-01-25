---
title: Тип ресурса governanceRoleSetting
description: " правила и т. д."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508169"
---
# <a name="governancerolesetting-resource-type"></a>Тип ресурса governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|resourceId           |String                                  |Обязательный. Идентификатор ресурса, с которым связана параметров ролей.|
|roleDefinitionId     |Строка                                  |Обязательный. Идентификатор определения роли, с которым связана параметров ролей.|
|isDefault            |Boolean                                 |Только для чтения. Укажите, является ли roleSetting roleSetting по умолчанию|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметров ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|lastUpdatedBy        |String                                  |Только для чтения. Отображаемое имя администратора, который последним обновил roleSetting.|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.|
|adminMemberSettings  |[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.|
|userEligibleSettings |[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли. Параметр не поддерживается в данный момент.|
|userMemberSettings   |[governanceRuleSetting](../resources/governancerulesetting.md) коллекции|Параметры правил, которые вычисляются при попытке активировать его назначения ролей.|

## <a name="relationships"></a>Отношения
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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
