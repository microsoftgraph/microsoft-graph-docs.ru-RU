---
title: Тип ресурса appHostedMediaConfig
description: Стек мультимедиа, размещенных в приложении.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 583964a6c7cd65ae4e8341f7fcba92d754916b36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884569"
---
# <a name="apphostedmediaconfig-resource-type"></a>Тип ресурса appHostedMediaConfig

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Стек мультимедиа, размещенных в приложении.

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| BLOB-объектов                              | Строка  | Blob конфигурации мультимедиа, созданные агентом смарт-мультимедиа.    |
| removeFromDefaultAudioGroup       | Логический | Удаление звук из группы по умолчанию звука                       |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appHostedMediaConfig"
}-->
```json
{
  "blob": "String",
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
