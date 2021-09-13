---
author: JeremyKelley
ms.date: 09/10/2017
title: Квота
ms.localizationpriority: medium
description: Ресурс quota предоставляет сведения об ограничениях дискового пространства в ресурсе Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71f0f29c4ab6979f7154940e9007665d020b7f68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143812"
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
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | Сведения о планах квоты на хранение диска. Только в личном OneDrive.|

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

