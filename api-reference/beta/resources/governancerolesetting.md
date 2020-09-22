---
title: Тип ресурса Говернанцеролесеттинг
description: Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 61889ef9f5ecd968b52704138260d3b39ceaf961
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081645"
---
# <a name="governancerolesetting-resource-type"></a>Тип ресурса Говернанцеролесеттинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей. Например, параметры роли могут включать правило "максимальная длительность назначения", правило "MFA Required on Activation" и т. д.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Перечисление](../api/governancerolesetting-list.md) | Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)|Перечисление коллекции параметров роли для ресурса.|
|[Получение](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Чтение свойств и связей параметра Role.|
|[Обновление](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Обновление объекта параметров роли. |

## <a name="properties"></a>Свойства
|Свойство               |Тип                                      |Описание|
|:--------------------|:---------------------------------------|:----------|
|id                   |Строка                                  |Идентификатор Ролесеттинг.|
|resourceId           |String                                  |Обязательный. Идентификатор ресурса, с которым связана Настройка роли.|
|роледефинитионид     |Строка                                  |Обязательный. Идентификатор определения роли, с которым связана Настройка роли.|
|isDefault            |Boolean                                 |Только для чтения. Указывает, является ли Ролесеттинг Ролесеттинг по умолчанию|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметра роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|ластупдатедби        |String                                  |Только для чтения. Отображаемое имя администратора, который последним обновил Ролесеттинг.|
|админелигиблесеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.|
|админмемберсеттингс  |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.|
|усерелигиблесеттингс |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли. Этот параметр не поддерживается в данный момент.|
|усермемберсеттингс   |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для этого параметра Role.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, принудительно заданное с помощью этого параметра роли. |

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


