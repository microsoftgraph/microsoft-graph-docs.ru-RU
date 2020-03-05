---
author: JeremyKelley
description: Ресурс Quota предоставляет сведения об ограничениях дискового пространства для ресурса Drive.
ms.date: 09/10/2017
title: Назначаем
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8421998d9815efcd23417aadde8ef29e28050647
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521287"
---
# <a name="quota-resource-type"></a>Тип ресурса Quota

Пространство имен: Microsoft. Graph

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
