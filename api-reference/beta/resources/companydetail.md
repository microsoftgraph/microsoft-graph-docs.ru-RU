---
title: Тип ресурса Компанидетаил
description: Тип ресурса Компанидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dc8da38c9da8d6631e8e46199f420ae0b3ab652e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507585"
---
# <a name="companydetail-resource-type"></a>Тип ресурса Компанидетаил

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о компаниях, связанных с сущностями в своем [профиле](profile.md).

## <a name="properties"></a>Свойства

| Свойство       | Тип                                | Описание                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|address         |[physicalAddress](physicaladdress.md)| Адрес компании.                     |
|department      |String                               | Название отдела в компании.           |
|displayName     |Строка                               | Название компании.                               |
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