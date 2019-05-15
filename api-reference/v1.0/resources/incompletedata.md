---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f26317cf16f0773852df35941c00e88df145cc31
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970815"
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
