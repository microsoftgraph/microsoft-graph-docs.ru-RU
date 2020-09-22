---
title: Тип ресурса Поситиондетаил
description: Тип ресурса Поситиондетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: fbd013292754dea43dd69b645dcd2ab735559b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971484"
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

