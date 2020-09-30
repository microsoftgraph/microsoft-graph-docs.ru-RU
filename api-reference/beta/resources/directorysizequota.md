---
title: Тип ресурса Директорисизекуота
description: Представляет используемую компанией общую квоту каталога.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8f5f172cb8f090b71b7e0fd3c89151668c167afd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315603"
---
# <a name="directorysizequota-resource-type"></a>Тип ресурса Директорисизекуота

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет используемую компанией общую квоту каталога.

## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|used|Int32| Использованная сумма квоты каталога. |
|total|Int32| Общая сумма квоты каталога.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
