---
author: psampath
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4c115276631c67cb796fd06c582dd490d4c59b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019476"
---
# <a name="storageplaninformation-resource-type"></a>Тип ресурса storagePlanInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **storagePlanInformation** предоставляет сведения о планах квот хранилища диска.

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

| Имя свойства     | Тип      | Описание                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| упградеаваилабле  | Boolean   | Указывает, доступны ли планы квоты хранилища выше. Только для чтения. |


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



