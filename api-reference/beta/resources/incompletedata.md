---
author: daspek
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
ms.date: 10/06/2017
title: инкомплетедата
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6505d02ee7436e02d90627cfd38a83e3e436706a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016568"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса Инкомплетедата

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.
Свойства, содержащиеся в, могут содержать сведения о причине неполных данных.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>Свойства

| Свойство                  | Тип           | Описание
|:--------------------------|:---------------|:--------------------------------
| миссингдатабефоредатетиме | DateTimeOffset | В службе нет исходных данных до указанного времени.
| вассроттлед              | Boolean        | Некоторые данные не были записаны из-за чрезмерной активности.

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


