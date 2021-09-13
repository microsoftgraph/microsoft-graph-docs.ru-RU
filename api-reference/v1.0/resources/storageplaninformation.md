---
author: learafa
description: Ресурс storagePlanInformation предоставляет сведения о планах квот на хранение диска.
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a26704495253d9dd33f4bcb37395b927ca8a4342
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136329"
---
# <a name="storageplaninformation-resource-type"></a>тип ресурса storagePlanInformation

Пространство имен: microsoft.graph

Предоставляет сведения о планах квоты на хранение диска.

## <a name="properties"></a>Свойства

| Имя свойства     | Тип      | Описание                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| **upgradeAvailable**  | Логический   | Указывает, существуют ли более высокие планы квоты на хранение. Только для чтения. |

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


