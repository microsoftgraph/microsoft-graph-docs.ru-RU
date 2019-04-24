---
title: Тип ресурса Говернанцеролесеттинг
description: " и т. д."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506321"
---
# <a name="governancerolesetting-resource-type"></a>Тип ресурса Говернанцеролесеттинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей. Например, параметры роли могут включать правило "максимальная длительность назначения", правило "MFA Required on Activation" и т. д.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)|ПереЧисление коллекции параметров роли для ресурса.|
|[получение](../api/governancerolesetting-get.md); |  [Говернанцеролесеттинг](../resources/governancerolesetting.md) |Чтение свойств и связей параметра Role.|
|[Обновление](../api/governancerolesetting-update.md) | [Говернанцеролесеттинг](../resources/governancerolesetting.md)  |Обновление объекта параметров роли. |

## <a name="properties"></a>Свойства
|Свойство               |Тип                                      |Описание|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |Идентификатор Ролесеттинг.|
|resourceId           |String                                  |Обязательный. Идентификатор ресурса, с которым связана Настройка роли.|
|Роледефинитионид     |String                                  |Обязательный. Идентификатор определения роли, с которым связана Настройка роли.|
|isDefault            |Boolean                                 |Только для чтения. Указывает, является ли Ролесеттинг Ролесеттинг по умолчанию|
|lastUpdatedDateTime  |DateTimeOffset                          |Только для чтения. Время последнего обновления параметра роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ластупдатедби        |String                                  |Только для чтения. Отображаемое имя администратора, который последним обновил Ролесеттинг.|
|Админелигиблесеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.|
|Админмемберсеттингс  |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.|
|Усерелигиблесеттингс |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли. Этот параметр не поддерживается в данный момент.|
|Усермемберсеттингс   |Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для этого параметра Role.|
|roleDefinition|[Говернанцероледефинитион](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, принудительно заданное с помощью этого параметра роли. |

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
