---
author: daspek
title: тип ресурса incompleteData
description: Аспект incompleteData указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b632148991aefd9fad09bd794e5f3e1849365af8cea5455bbef0ba628b60f221
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223580"
---
# <a name="incompletedata-resource-type"></a>тип ресурса incompleteData

Пространство имен: microsoft.graph

Аспект **incompleteData** указывает, что ресурс был создан с неполными данными.
Свойства внутри могут предоставлять сведения о том, почему данные являются неполными.

## <a name="properties"></a>Свойства

| Свойство                  | Тип           | Описание
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | Служба не имеет исходных данных до указанного времени.
| wasThrottled              | Логический        | Некоторые данные не были записаны из-за чрезмерной активности.

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

