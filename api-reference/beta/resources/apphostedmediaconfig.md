---
title: Тип ресурса Апфостедмедиаконфиг
description: Стек мультимедиа, размещенный в приложении.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abc9cd8aa916c4e0b9141f79151fbd7e9f2d3b8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013369"
---
# <a name="apphostedmediaconfig-resource-type"></a>Тип ресурса Апфостедмедиаконфиг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Стек мультимедиа, размещенный в приложении.

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| характеристики                              | String  | Большой двоичный объект конфигурации мультимедиа, созданный агентом интеллектуальных носителей.    |
| Ремовефромдефаултаудиограуп       | Boolean | Удаление звука из группы "звук" по умолчанию                       |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
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
<!--
{
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
