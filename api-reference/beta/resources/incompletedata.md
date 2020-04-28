---
author: daspek
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
ms.date: 10/06/2017
title: инкомплетедата
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 3abefff4749413648a3f1a56d1dbf6d44f16a471
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496280"
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
