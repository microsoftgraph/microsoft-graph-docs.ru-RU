---
author: daspek
title: Тип ресурса incompleteData
description: Аспект incompleteData указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 20dda8e9d1cd321a465c7a257cb5cb7bed845351
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239935"
---
# <a name="incompletedata-resource-type"></a>Тип ресурса incompleteData

Пространство имен: microsoft.graph

Аспект **incompleteData указывает,** что ресурс был создан с неполными данными.
Свойства внутри могут предоставлять сведения о том, почему данные неполные.

## <a name="properties"></a>Свойства

| Свойство                  | Тип           | Описание
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | Служба не имеет исходных данных до указанного времени.
| wasThrottled              | Логическое        | Некоторые данные не были записаны из-за чрезмерной активности.

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

