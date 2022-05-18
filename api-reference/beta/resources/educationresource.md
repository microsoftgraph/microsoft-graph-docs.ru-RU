---
title: Тип ресурса educationResource
description: Базовый класс для всех объектов ресурсов в системе.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1af5cb6ae12eb435b6335d902430fdbc717fcd25
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461368"
---
# <a name="educationresource-resource-type"></a>Тип ресурса educationResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовый класс для [educationExcelResource](../resources/educationexcelresource.md), [educationFileResource](../resources/educationfileresource.md), [educationLinkResource](../resources/educationlinkresource.md), [educationPowerPointResource](../resources/educationpowerpointresource.md), [educationWordResource](../resources/educationwordresource.md), [educationMediaResource](../resources/educationmediaresource.md), [educationExternalResource](../resources/educationexternalresource.md) и [educationTeamsAppResource](../resources/educationteamsappresource.md).

Объект educationResource связан с назначением [](educationassignment.md) и (или) [отправкой, которая](educationsubmission.md) представляет обучающий объект, который передается или передается. Создание экземпляра ресурса напрямую невозможно; Необходимо создать подкласс, который будет представлять тип используемого ресурса.

Этот ресурс хранит общие свойства для всех типов ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Кто создали ресурс.|
|createdDateTime|Момент времени создания ресурса.  DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|displayName|String|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Кто последним пользователем, который изменяет ресурс.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


