---
title: Тип ресурса governanceRoleSetting
description: Представляет набор конфигураций для каждого определения роли, который необходимо оценить при создании или изменении назначений ролей.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: d5e441b35cd4b6ccdb52710508bd8afe5955d860
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399470"
---
# <a name="governancerolesetting-resource-type"></a>Тип ресурса governanceRoleSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет набор конфигураций для каждого определения роли, который необходимо оценить при создании или изменении назначений ролей. Например, параметры роли могут включать правило "максимальная длительность назначения", правило MFA, необходимое для активации, и т. д.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Перечисление](../api/governancerolesetting-list.md) | [Коллекция governanceRoleSetting](../resources/governancerolesetting.md)|Вывод списка параметров роли для ресурса.|
|[Получение](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Чтение свойств и связей параметра роли.|
|[Обновление](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Обновление объекта параметра роли. |

## <a name="properties"></a>Свойства
|Свойство               |Тип                                      |Описание|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |Идентификатор roleSetting.|
|resourceId           |String                                  |Обязательный. Идентификатор ресурса, с помощью которого связан параметр роли.|
|roleDefinitionId     |String                                  |Обязательный. Идентификатор определения роли, с помощью которого связан параметр роли.|
|isDefault            |Boolean                                 |Только для чтения. Укажите, является ли roleSetting ролью по умолчанию.|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметра роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastUpdatedBy        |String                                  |Только для чтения. Отображаемое имя администратора, который последним обновил roleSetting.|
|adminEligibleSettings|[Коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытке администратора добавить допустимое назначение роли.|
|adminMemberSettings  |[Коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правила, которые оцениваются при попытке администратора добавить назначение роли прямого участника.|
|userEligibleSettings |[Коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается добавить допустимое назначение роли. Этот параметр пока не поддерживается.|
|userMemberSettings   |[Коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правила, которые оцениваются, когда пользователь пытается активировать назначение роли.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для этого параметра роли.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, которое применяется с этим параметром роли. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->


