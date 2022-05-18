---
title: Тип ресурса educationTeamsAppResource
description: Соответствует [установленному Microsoft Teams приложения](teamsappinstallation.md). Это позволяет пользователям образовательных служб создавать задания и совместно использовать их с внедренными Teams приложениями.
author: adarshgh
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a3f77be2aa1a5e6566b8d216735138da2daab8c3
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461821"
---
# <a name="educationteamsappresource-resource-type"></a>Тип ресурса educationTeamsAppResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Образовательный ресурс, соответствующий [установленному Microsoft Teams приложения](teamsappinstallation.md). Это позволяет пользователям образовательных служб создавать задания и совместно использовать их с внедренными Teams приложениями, такими как YouTube или FlipGrid.

Сведения об использовании FlipGrid для образовательных Microsoft Teams см. в [статье о FlipGrid](https://education.microsoft.com/en-us/resource/13cb22b1).

Наследуется от [educationResource](educationresource.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|string|Отображаемое имя ресурса.|
|appId|string|Teams идентификатор приложения.|
|appIconWebUrl|string|URL-адрес, указывающий на значок приложения.|
|teamsEmbeddedContentUrl|string|URL-адрес ресурса приложения, который будет открыт Teams.|
|webUrl|string|URL-адрес ресурса приложения, который можно открыть в браузере.|
|createdBy|String|Отображаемое имя пользователя, создавшего этот ресурс. Наследуется от **educationResource**.|
|createdDateTime|DateTimeOffset|Дата, когда была добавлена повторная ошибка. Наследуется от **educationResource**.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменяет ресурс. Наследуется от **educationResource**.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения ресурса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Наследуется от **educationResource**.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeamsAppResource"
}-->

```json
{
  "displayName": "String",
  "appId": "Unique String",
  "appIconWebUrl": "String URL",
  "teamsEmbeddedContentUrl": "String URL",
  "webUrl": "String URL",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


