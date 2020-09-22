---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 424a857468473532dc6f2a39c4c13dc94b52406c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054891"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса Инкомплетедата

Пространство имен: microsoft.graph

Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.
В свойствах могут содержаться сведения о причине неполных данных.

## <a name="properties"></a>Свойства

| Свойство                  | Тип           | Описание
|:--------------------------|:---------------|:--------------------------------
| миссингдатабефоредатетиме | DateTimeOffset | В службе нет исходных данных до указанного времени.
| вассроттлед              | Boolean        | Некоторые данные не были записаны из-за чрезмерной активности.

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

