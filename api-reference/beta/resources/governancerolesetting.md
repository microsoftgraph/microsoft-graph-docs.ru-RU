---
title: тип ресурса governanceRoleSetting
description: Представляет набор конфигураций для каждого определения ролей, которые необходимо оценивать при назначении ролей при их назначении или изменениях.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 8a98725d26d160b9d8687fceb87e6811440ed31a
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509660"
---
# <a name="governancerolesetting-resource-type"></a>тип ресурса governanceRoleSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет набор конфигураций для каждого определения ролей, которые необходимо оценивать при назначении ролей при их назначении или изменениях. Например, параметры ролей могут включать правило "максимальная продолжительность назначения", правило "MFA, требуемая для активации" и так далее.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Список](../api/governancerolesetting-list.md) | [коллекция governanceRoleSetting](../resources/governancerolesetting.md)|Список параметров ролей на ресурсе.|
|[Получение](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Чтение свойств и связей параметра ролей.|
|[обновление](../api/governancerolesetting-update.md). | [governanceRoleSetting](../resources/governancerolesetting.md)  |Обновление объекта параметра роли. |

## <a name="properties"></a>Свойства
|Свойство               |Тип                                      |Описание|
|:--------------------|:---------------------------------------|:----------|
|id                   |Строка                                  |Id of the roleSetting.|
|resourceId           |String                                  |Обязательный. ID ресурса, с который связан параметр роли.|
|roleDefinitionId     |String                                  |Обязательный. ID определения роли, с чем связан параметр роли.|
|isDefault            |Boolean                                 |Только для чтения. Указать, является ли рольSetting ролью по умолчанию.|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметра роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastUpdatedBy        |String                                  |Только для чтения. Отображает имя администратора, который в последний раз обновлял рольSetting.|
|adminEligibleSettings|[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при добавлении администратором назначения подходящих ролей.|
|adminMemberSettings  |[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда администратор пытается добавить назначение ролей прямого участника.|
|userEligibleSettings |[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, оцениваемые при добавлении права на назначение ролей. Параметр пока не поддерживается.|
|userMemberSettings   |[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытках пользователя активировать назначение ролей.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для этого параметра ролей.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, которое выполняется с помощью этого параметра роли. |

## <a name="json-representation"></a>Представление JSON

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


