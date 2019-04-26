---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Инкомплетедата
localization_priority: Normal
ms.openlocfilehash: 40c1b782384076eefc986f67dc1736f191feb7b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339969"
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
| Вассроттлед              | Логический        | Некоторые данные не были записаны из-за чрезмерной активности.

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
