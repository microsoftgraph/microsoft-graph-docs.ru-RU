---
title: regionalFormatOverrides resource type
description: Ресурс, представляющий переопределения региональных форматов для календарей, дат и времени.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2b4046ad8ec6b2d646d1dc2d93cbe7bed205cbad
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516071"
---
# <a name="regionalformatoverrides-resource-type"></a>regionalFormatOverrides resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция строк, представляющих переопределения форматирования для календарей, дат и времени. 

## <a name="properties"></a>Свойства

|Свойство             |Тип                     |Описание                                                    |
|---------------------|-------------------------|---------------------------------------------------------------|
|calendar             |String                   |Календарь для использования, например, григорианский календарь.<br><br>Возвращается по умолчанию.|                   
|firstDayOfWeek       |microsoft.graph.dayOfWeek|Первый день недели в использовании, например, воскресенье.<br><br>Возвращается по умолчанию.|
|shortDateFormat      |String                   |Короткий формат времени даты, который будет использоваться для отображения дат.<br><br>Возвращается по умолчанию.|
|longDateFormat       |String                   |Формат времени даты, используемый для отображения дат.<br><br>Возвращается по умолчанию.|
|shortTimeFormat      |String                   |Короткий формат времени, который будет использоваться для отображения времени.<br><br>Возвращается по умолчанию.|
|longTimeFormat       |String                   |Формат длительного времени, который будет использоваться для отображения времени.<br><br>Возвращается по умолчанию.|
|timeZone             |String                   |Часовой пояс, используемый для отображения времени.<br><br>Возвращается по умолчанию.|

## <a name="json-representation"></a>Представление JSON

Ниже приводится определение ресурса JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.regionalFormatOverrides"
}-->

```json
{
    "calendar": "string",
    "firstDayOfWeek": "string",
    "shortDateFormat": "string",
    "longDateFormat": "string",
    "shortTimeFormat": "string",
    "longTimeFormat": "string",
    "timeZone": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalFormatOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


