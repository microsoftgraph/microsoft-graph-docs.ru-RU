---
title: Тип ресурса Апфостедмедиаконфиг
description: Стек мультимедиа, размещенный в приложении.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0cb34d0673404c90607a8f1ac442ca1b7c504ce9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339183"
---
# <a name="apphostedmediaconfig-resource-type"></a>Тип ресурса Апфостедмедиаконфиг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Стек мультимедиа, размещенный в приложении.

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| характеристики                              | String  | Большой двоичный объект конфигурации мультимедиа, созданный агентом интеллектуальных носителей.    |
| Ремовефромдефаултаудиограуп       | Логический | Удаление звука из группы "звук" по умолчанию                       |

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
