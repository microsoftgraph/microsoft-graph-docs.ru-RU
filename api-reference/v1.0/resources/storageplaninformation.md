---
author: learafa
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: b8b4778a4726c227bfe79ad13ecb14507b13a889
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036956"
---
# <a name="storageplaninformation-resource-type"></a>Тип ресурса storagePlanInformation

Пространство имен: microsoft.graph

Предоставляет сведения о планах квот хранилища диска.

## <a name="properties"></a>Свойства

| Имя свойства     | Тип      | Описание                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| **упградеаваилабле**  | Boolean   | Указывает, доступны ли планы квоты для хранилища выше. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```

<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->


