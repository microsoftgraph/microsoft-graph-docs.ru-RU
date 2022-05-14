---
author: daspek
description: Аспект incompleteData указывает, что ресурс был создан с неполными данными.
ms.date: 10/06/2017
title: IncompleteData
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: b24b10db7f38ee17356c77d40bcda3b08576e45b
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420679"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса incompleteData

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аспект **incompleteData указывает** , что ресурс был создан с неполными данными.
Свойства внутри могут предоставлять сведения о том, почему имеются неполные данные.

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
| missingDataBeforeDateTime | DateTimeOffset | Служба не имеет исходных данных до указанного времени.
| wasThrottled              | Логический        | Некоторые данные не были записаны из-за чрезмерной активности.

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


