---
title: сложный тип Интерналспонсорс
description: Определяет связь с другим пользователем в клиенте, который будет разрешен в качестве утверждающего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c7ec468638de5e9a49cbf2f664eb7d05e3bef5b1
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331480"
---
# <a name="internalsponsors-complex-type"></a>сложный тип Интерналспонсорс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется на этапе утверждения [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Это подтип набора [пользователей](userset.md), в котором `@odata.type` значение `#microsoft.graph.internalSponsors` указывает на то, что пользователь, подключенный к Организации, может быть утверждающим в качестве внутреннего спонсора. Этот утверждающий применяется только к запросам пользователей, которые являются частью подключенной Организации.  При создании этапа утверждения политики назначения пакетов Access с Интерналспонсорс также включает другой утверждающий, например одного пользователя или члена группы, если у подключенной Организации нет внутреннего спонсора.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| Создание резервной копии | Логический | Указывает, является ли спонсор резервным утверждающим. |

## <a name="json-representation"></a>Представление JSON

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
