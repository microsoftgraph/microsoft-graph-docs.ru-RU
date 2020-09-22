---
title: Тип ресурса Регионалформатоверридес
description: Ресурс, представляющий региональные параметры форматирования для календарей, дат и времени.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 2ed130135571faeced90a638e9334a7e2a185a5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073514"
---
# <a name="regionalformatoverrides-resource-type"></a>Тип ресурса Регионалформатоверридес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция строк, представляющих переопределения форматирования для календарей, дат и времени. 

## <a name="properties"></a>Свойства

|Свойство             |Тип                 |Описание                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|calendar             |String               |Используемый календарь, например, григорианский календарь.<br><br>Возвращается по умолчанию.|                   
|firstDayOfWeek       |String               |Первый день недели, который необходимо использовать, например, воскресенье.<br><br>Возвращается по умолчанию.|
|шортдатеформат      |String               |Краткий формат даты и времени, используемый для отображения дат.<br><br>Возвращается по умолчанию.|
|лонгдатеформат       |String               |Длинный формат даты и времени, используемый для отображения дат.<br><br>Возвращается по умолчанию.|
|шорттимеформат      |String               |Краткий формат времени, используемый для отображения времени.<br><br>Возвращается по умолчанию.|
|лонгтимеформат       |String               |Длинный формат времени, используемый для отображения времени.<br><br>Возвращается по умолчанию.|
|timeZone             |String               |Часовой пояс, используемый для отображения времени.<br><br>Возвращается по умолчанию.|

## <a name="json-representation"></a>Представление JSON

Ниже приведено определение ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "",
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


