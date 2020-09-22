---
author: JeremyKelley
description: Ресурс Quota предоставляет сведения об ограничениях дискового пространства для ресурса Drive.
ms.date: 09/10/2017
title: Назначаем
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9477662c1ffa8419d7be293c31b8f50b06bd74d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993058"
---
# <a name="quota-resource-type"></a>Тип ресурса Quota

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Quota** предоставляет сведения об ограничениях [дискового](drive.md) пространства для ресурса Drive.

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
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | Сведения о планах квот хранилища диска. Только в личном хранилище OneDrive.|

### <a name="state-enumeration-values"></a>Значения перечисления State

| Значение      | Описание                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | На диске еще много свободного дискового пространства.                                                                                                                               |
| `nearing`  | Объем свободного дискового пространства менее 10 % общего объема дискового пространства.                                                                                                                      |
| `critical` | Объем свободного дискового пространства менее 1 % общего объема дискового пространства.                                                                                                                       |
| `exceeded` | Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство. |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->


