---
author: JeremyKelley
ms.date: 09/10/2017
title: Quota
localization_priority: Normal
description: Ресурс quota предоставляет сведения об ограничениях дискового пространства в ресурсе Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 145d145e764128c719e757c213b8d7b2266e0b68
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238899"
---
# <a name="quota-resource-type"></a>Тип ресурса quota

Пространство имен: microsoft.graph

Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | Общий объем разрешенного дискового пространства в байтах. Только для чтения.                           |
| used          | Int64  | Общий объем использованного дискового пространства в байтах. Только для чтения.                                      |
| remaining     | Int64  | Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения. |
| deleted       | Int64  | Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.      |
| состояние         | string | Значение перечисления, указывающее состояние дискового пространства. Только для чтения. |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | Сведения о планах квот дискового пространства. Только в Личном хранилище OneDrive.|

## <a name="state-enumeration"></a>Перечисление state

| Значение      | Описание                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | На диске еще много свободного дискового пространства.                                                                                                                               |
| `nearing`  | Объем свободного дискового пространства менее 10 % общего объема дискового пространства.                                                                                                                      |
| `critical` | Объем свободного дискового пространства менее 1 % общего объема дискового пространства.                                                                                                                       |
| `exceeded` | Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство. |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->

