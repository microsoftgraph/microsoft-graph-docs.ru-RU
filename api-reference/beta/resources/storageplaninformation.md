---
author: psampath
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 79254efa033528bd8fd4cf66a07959a71e3fef1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520438"
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

