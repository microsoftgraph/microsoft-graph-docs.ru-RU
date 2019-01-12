---
title: Тип ресурса appHostedMediaConfig
description: Стек мультимедиа, размещенных в приложении.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 36f869be347e2d55ec90079c62c5b6ebef85f144
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928586"
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
