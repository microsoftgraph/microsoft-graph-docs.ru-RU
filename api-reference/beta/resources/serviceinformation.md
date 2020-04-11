---
title: Тип ресурса Сервицеинформатион
description: Тип ресурса Сервицеинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: daca733578e5415fc777bc01a8ef1272cfdcc681
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228882"
---
# <a name="serviceinformation-resource-type"></a>Тип ресурса Сервицеинформатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовые описательные данные о облачных службах, на которые пользователь выбрал ссылку из своей учетной записи.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|name          | String      | Имя облачной службы (например, Twitter, Инстаграм). |
|webUrl        | String      | Содержит URL-адрес для службы, на которую указывает ссылка.               |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
