---
title: Тип ресурса appHostedMediaConfig
description: Стек мультимедиа, размещенных в приложении.
ms.openlocfilehash: 39080a8fdb5688ed9f1a5a8daba43266a0e7003e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076107"
---
# <a name="apphostedmediaconfig-resource-type"></a>Тип ресурса appHostedMediaConfig

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Стек мультимедиа, размещенных в приложении.

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Description                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| BLOB-объектов                              | String  | Blob конфигурации мультимедиа, созданные агентом смарт-мультимедиа.    |
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
