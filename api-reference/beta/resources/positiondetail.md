---
title: Тип ресурса Поситиондетаил
description: Тип ресурса Поситиондетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6c77c116f013000ec4d419ec20c1e45c07187a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521595"
---
# <a name="positiondetail-resource-type"></a>Тип ресурса Поситиондетаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о позициях, связанных с сущностями в [профиле](profile.md)пользователя.

## <a name="properties"></a>Свойства

| Свойство       | Тип                             | Описание                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|внутрихолдинговом         |[компанидетаил](companydetail.md) | Подробные сведения о компании или работодателе.                  |
|description     |String                            | Описание интересующей должности.               |
|ендмонсеар    |Дата                              | По завершении должности.                               |
|jobTitle;        |String                            | Заголовок, хранящийся в этой позиции.                  |
|role            |String                            | Роль, к которой присвоено место.                        |
|стартмонсеар  |Дата                              | Начальный месяц и год позиции.              |
|summary         |String                            |Краткое описание положения.                          |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->