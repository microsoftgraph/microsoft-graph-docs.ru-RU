---
title: Тип ресурса Говернанцеролесеттинг
description: " и т. д."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1bd1821bbb3336386b54b62ebe7b4787c85d1ebf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006425"
---
# <a name="governancerolesetting-resource-type"></a>Тип ресурса Говернанцеролесеттинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей. Например, параметры роли могут включать правило "максимальная длительность назначения", правило "MFA Required on Activation" и т. д.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)|Перечисление коллекции параметров роли для ресурса.|
|[получение](../api/governancerolesetting-get.md); |  [Говернанцеролесеттинг](../resources/governancerolesetting.md) |Чтение свойств и связей параметра Role.|
|[обновление](../api/governancerolesetting-update.md); | [Говернанцеролесеттинг](../resources/governancerolesetting.md)  |Обновление объекта параметров роли. |

## <a name="properties"></a>Свойства
|Свойство               |Тип                                      |Описание|
|:--------------------|:---------------------------------------|:----------|
|id                   |Строка                                  |Идентификатор Ролесеттинг.|
|resourceId           |String                                  |Обязательный. Идентификатор ресурса, с которым связана Настройка роли.|
|Роледефинитионид     |String                                  |Обязательный. Идентификатор определения роли, с которым связана Настройка роли.|
|isDefault            |Boolean                                 |Только для чтения. Указывает, является ли Ролесеттинг Ролесеттинг по умолчанию|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметра роли. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ластупдатедби        |String                                  |Только для чтения. Отображаемое имя администратора, который последним обновил Ролесеттинг.|
|Админелигиблесеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.|
|Админмемберсеттингс  |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.|
|Усерелигиблесеттингс |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли. Этот параметр не поддерживается в данный момент.|
|Усермемберсеттингс   |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для этого параметра Role.|
|roleDefinition|[Говернанцероледефинитион](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, принудительно заданное с помощью этого параметра роли. |

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
