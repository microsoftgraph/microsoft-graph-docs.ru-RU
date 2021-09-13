---
title: тип ресурса serviceHostedMediaConfig
description: Тип serviceHostedMediaConfig.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8179b27817627b95925e3ab84c3ea5b84b57d119
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126669"
---
# <a name="servicehostedmediaconfig-resource-type"></a>тип ресурса serviceHostedMediaConfig

Пространство имен: microsoft.graph

Средства массовой информации, которые хозяйские удаленно. Это наследуется [от mediaConfig](mediaconfig.md).

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                        | Описание                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| preFetchMedia               | [коллекция mediaInfo](mediainfo.md)                        | Список мультимедиа для предварительного получения.                   |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

