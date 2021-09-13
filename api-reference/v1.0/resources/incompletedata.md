---
author: daspek
title: тип ресурса incompleteData
description: Аспект incompleteData указывает, что ресурс был создан с неполными данными.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f4d8c852a08780ecc0f48ac8a1dcef11b246673c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128314"
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

