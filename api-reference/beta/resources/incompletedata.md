---
author: daspek
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
ms.date: 10/06/2017
title: Инкомплетедата
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006285"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса Инкомплетедата

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
| Миссингдатабефоредатетиме | DateTimeOffset | В службе нет исходных данных до указанного времени.
| Вассроттлед              | Boolean        | Некоторые данные не были записаны из-за чрезмерной активности.

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
