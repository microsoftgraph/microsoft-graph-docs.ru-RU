---
title: Тип ресурса appHostedMediaConfig
description: Стек мультимедиа, размещенных в приложении.
author: VinodRavichandran
ms.openlocfilehash: b96d6ff836ab36e5561c9ba3958123178e2fbde9
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380130"
---
# <a name="apphostedmediaconfig-resource-type"></a>Тип ресурса appHostedMediaConfig

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Стек мультимедиа, размещенных в приложении.

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| BLOB-объектов                              | String  | Blob конфигурации мультимедиа, созданные агентом смарт-мультимедиа.    |
| removeFromDefaultAudioGroup       | Boolean | Удаление звук из группы по умолчанию звука                       |

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
