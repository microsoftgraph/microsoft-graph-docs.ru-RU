---
author: psampath
description: Ресурс storagePlanInformation предоставляет сведения о планах квот на хранение диска.
ms.date: 06/20/2018
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: db5707686f6104d8d9004696094c0bcc22066f5a
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723272"
---
# <a name="storageplaninformation-resource-type"></a>тип ресурса storagePlanInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **storagePlanInformation** предоставляет сведения о планах квот на хранение диска.

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
| upgradeAvailable | Boolean | Указывает, имеются ли более высокие планы квоты на хранение. Только для чтения. |

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
