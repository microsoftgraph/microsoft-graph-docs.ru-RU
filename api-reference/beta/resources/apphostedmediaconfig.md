---
title: Тип ресурса Апфостедмедиаконфиг
description: Стек мультимедиа, размещенный в приложении.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 70bd631631dd5d4fdebe55d379ea61f98fba19a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508312"
---
# <a name="apphostedmediaconfig-resource-type"></a>Тип ресурса Апфостедмедиаконфиг

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Стек мультимедиа, размещенный в приложении.

## <a name="properties"></a>Свойства

| Свойство                          | Тип    | Описание                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| характеристики                              | String  | Большой двоичный объект конфигурации мультимедиа, созданный агентом интеллектуальных носителей.    |
| ремовефромдефаултаудиограуп       | Логический | Удаление звука из группы "звук" по умолчанию                       |

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
