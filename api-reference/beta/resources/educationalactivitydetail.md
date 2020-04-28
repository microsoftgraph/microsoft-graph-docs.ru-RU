---
title: Тип ресурса Едукатионалактивитидетаил
description: Тип ресурса Едукатионалактивитидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ccacf02184bbf54e49949d7671d34dde93b3859f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502825"
---
# <a name="educationalactivitydetail-resource-type"></a>Тип ресурса Едукатионалактивитидетаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет дополнительные сведения о выпуске, выпускнике, степени выпуске или других образовательных действиях, выполняемых пользователем и используемом в ресурсе [едукатионалактивити](educationalActivity.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|Аббревиатура  |String       |Сокращенное название степени или программы (пример: "доктор", "МБА")    |
|activities    |String       |Действия факультативных, выполняемые вместе с программой.   |
|Награды        |String       |Любые награды или соблюдаются, связанные с программой.              |
|description   |Строка       |Краткое описание программы, предоставленной пользователем.         |
|displayName   |Строка       |Длинное имя программы, предоставленной пользователем.      |
|фиелдсофстуди |String       |Основной и дополнительный номера, связанные с программой. (если это необходимо) |
|оценка         |String       |Конечный уровень, класс, GPA или оценка.                          |
|notes         |String       |Дополнительные примечания, предоставленные пользователем.                        |
|webUrl        |String       |Ссылка на страницу "степень" или "программа".                            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivityDetail",
  "baseType": null
}-->

```json
{
  "abbreviation": "String",
  "activities": "String",
  "awards": "String",
  "description": "String",
  "displayName": "String",
  "fieldsOfStudy": "String",
  "grade": "String",
  "notes": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivityDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->