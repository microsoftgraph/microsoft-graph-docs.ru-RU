---
title: Тип ресурса audioDuckingConfiguration
description: Параметры для Уклонение от других источников, (синхронизацию и выходить из нее других источников).
author: VinodRavichandran
ms.openlocfilehash: e595e2a46f3e8bcbee2bb7ad0e3421216244db71
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380182"
---
# <a name="audioduckingconfiguration-resource-type"></a>Тип ресурса audioDuckingConfiguration

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Параметры для Уклонение от других источников, (синхронизацию и выходить из нее других источников).

## <a name="properties"></a>Свойства

| Свойство      | Тип     | Описание                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | Объем источников в процентах, когда источники которые ducked.             |
| rampActive    | Int64    | Количество времени (в миллисекундах), необходимое для ducked источников, чтобы «сделать». |
| rampInactive  | Int64    | Количество времени (в миллисекундах), необходимое для ducked источников «увеличение».  |
| upperLevel    | Int64    | Объем источников в процентах, когда ducked источников не выполняется.         |

> **Примечание:** Продолжительность расширение путь не может быть более 5000 миллисекунд.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
