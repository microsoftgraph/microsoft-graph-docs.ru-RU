---
title: " Тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076110"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса averageComparativeScore

Этот ресурс содержит различные различных показателям на основе, различные области (например, среднее число по вертикали отрасли, Средний размер рабочее место компании и т. п.) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры).

|Свойство |Тип |Description |
|:--|:--|:--|
|   Основы   |   String  |   Тип области (с AllTenants, Общее_число_мест, IndustryTypes).  |
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
