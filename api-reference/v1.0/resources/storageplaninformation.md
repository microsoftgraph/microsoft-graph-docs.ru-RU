---
author: learafa
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a5e6c10bdbc8a68230a223501844d0ee121014c2
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863777"
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

