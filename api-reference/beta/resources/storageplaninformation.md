---
author: psampath
description: Ресурс storagePlanInformation предоставляет сведения о планах квоты хранилища диска.
ms.date: 06/20/2018
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 036da4561666bacf12f3cd7a448c9b9ba18808aa
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735945"
---
# <a name="storageplaninformation-resource-type"></a>Тип ресурса storagePlanInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **storagePlanInformation** предоставляет сведения о планах квоты хранилища диска.

### <a name="json-representation"></a>Представление JSON

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

## <a name="properties"></a>Свойства

| Свойство         | Тип    | Описание                                                             |
| :--------------- | :------ | :---------------------------------------------------------------------- |
| upgradeAvailable | Логический | Указывает, существуют ли более высокие планы квоты хранилища. Только для чтения. |

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
