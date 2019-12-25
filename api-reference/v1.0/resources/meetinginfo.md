---
title: Тип ресурса Митингинфо
description: Сведения о собрании, указанные для создания или присоединения к собранию.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e777de1b9f6710156106ce8dab5704613b98e1e5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871393"
---
# <a name="meetinginfo-resource-type"></a>Тип ресурса Митингинфо

Это абстрактный класс, который содержит сведения о собрании.
 
Чтобы присоединиться к существующему собранию, необходимо либо указать [организермитингинфо](organizermeetinginfo.md) в сочетании с [чатинфо](./chatinfo.md), либо только с [токенмитингинфо](tokenmeetinginfo.md).


## <a name="derived-types"></a>Производные типы

| Тип                                                 | Описание                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [организермитингинфо](./organizermeetinginfo.md)    | Сведения об организаторе собрания                          |
| [токенмитингинфо](tokenmeetinginfo.md)              | Зашифрованный маркер, содержащий сведения о собрании  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
