---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029241"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса Инкомплетедата

Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.
В свойствах могут содержаться сведения о причине неполных данных.

## <a name="properties"></a>Свойства

| Свойство                  | Тип           | Описание
|:--------------------------|:---------------|:--------------------------------
| Миссингдатабефоредатетиме | DateTimeOffset | В службе нет исходных данных до указанного времени.
| Вассроттлед              | Boolean        | Некоторые данные не были записаны из-за чрезмерной активности.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
