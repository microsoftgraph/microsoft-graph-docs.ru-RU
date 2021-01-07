---
title: Тип ресурса regionalFormatOverrides
description: Ресурс, представляющий переопределения регионального форматирования для календарей, дат и времени.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 437b67f6a99017bb20096dbd20451b7662145cbd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777598"
---
# <a name="regionalformatoverrides-resource-type"></a>Тип ресурса regionalFormatOverrides

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция строк, представляющих переопределения форматирования для календарей, дат и времени. 

## <a name="properties"></a>Свойства

|Свойство             |Тип                 |Описание                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|calendar             |String               |Календарь, который необходимо использовать, например григорианский календарь.<br><br>Возвращается по умолчанию.|                   
|firstDayOfWeek       |String               |Первый день недели, например воскресенье.<br><br>Возвращается по умолчанию.|
|shortDateFormat      |String               |Краткий формат даты и времени, используемый для отображения дат.<br><br>Возвращается по умолчанию.|
|longDateFormat       |String               |Длинный формат даты и времени, используемый для отображения дат.<br><br>Возвращается по умолчанию.|
|shortTimeFormat      |String               |Короткий формат времени, используемый для отображения времени.<br><br>Возвращается по умолчанию.|
|longTimeFormat       |String               |Длинный формат времени, используемый для отображения времени.<br><br>Возвращается по умолчанию.|
|timeZone             |String               |Часовой пояс, используемый для отображения времени.<br><br>Возвращается по умолчанию.|

## <a name="json-representation"></a>Представление JSON

Ниже приводится определение ресурса в JSON.

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


