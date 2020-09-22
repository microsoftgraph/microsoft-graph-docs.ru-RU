---
title: сложный тип Интерналспонсорс
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56ae53e1b55be0a56a4c021449b8c5f4eb1a7c05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058392"
---
# <a name="internalsponsors-complex-type"></a>сложный тип Интерналспонсорс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется на этапе утверждения [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.internalSponsors` указывает на то, что пользователь, подключенный к Организации, может быть утверждающим в качестве внутреннего спонсора. Этот утверждающий применяется только к запросам пользователей, которые являются частью подключенной Организации.  При создании этапа утверждения политики назначения пакетов Access с Интерналспонсорс также включает другой утверждающий, например одного пользователя или члена группы, если у подключенной Организации нет внутреннего спонсора.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| Создание резервной копии | Boolean | Указывает, является ли спонсор резервным утверждающим. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


