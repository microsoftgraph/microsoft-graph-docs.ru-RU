---
title: " Тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834596"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса averageComparativeScore

Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   Основы   |   Строка  |   Тип области (с AllTenants, Общее_число_мест, IndustryTypes).  |
|   «СреднийБалл»    |   Double  | Средняя оценка в рамках указанного основы. |
|   deviceScore |   Double  | Средняя оценка в рамках указанного основы. |
|   dataScore   |   Double  | Средняя оценка в рамках указанного основы. |
|   identityScore   |   Double  | Средняя оценка в рамках указанного основы. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
