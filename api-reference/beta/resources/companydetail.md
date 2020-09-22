---
title: Тип ресурса Компанидетаил
description: Тип ресурса Компанидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 93b5490048c149ca526a9c3d0024175c1c20d7e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033932"
---
# <a name="companydetail-resource-type"></a>Тип ресурса Компанидетаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о компаниях, связанных с сущностями в своем [профиле](profile.md).

## <a name="properties"></a>Свойства

| Свойство       | Тип                                | Описание                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|address         |[physicalAddress](physicaladdress.md)| Адрес компании.                     |
|department      |String                               | Название отдела в компании.           |
|displayName     |String                               | Название компании.                               |
|officeLocation  |String                               | Местонахождение комнаты для пользователя, на который ссылается.  |
|произношение   |String                               | Рекомендации по произношению названия компании.   |
|webUrl          |String                               | Ссылка на домашнюю страницу компании.              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

