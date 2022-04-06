---
author: JeremyKelley
description: Ресурс квоты содержит сведения о ограничениях пространства на ресурсе диска.
ms.date: 09/10/2017
title: Квота
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 28006748084878d5c7ce3f327f6c4237e12bf83c
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722435"
---
# <a name="quota-resource-type"></a>тип ресурсов квоты

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **квоты** содержит сведения о ограничениях пространства на [ресурсе диска](drive.md) .

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

| Свойство               | Тип                                                | Описание                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------- |
| total                  | Int64                                               | Общий объем разрешенного дискового пространства в байтах. Только для чтения.                             |
| used                   | Int64                                               | Общий объем использованного дискового пространства в байтах. Только для чтения.                                        |
| remaining              | Int64                                               | Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.   |
| deleted                | Int64                                               | Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.        |
| состояние                  | string                                              | Значение перечисления, указывающее состояние дискового пространства. Только для чтения.   |
| storagePlanInformation | [storagePlanInformation](storageplaninformation.md) | Сведения о планах квоты на хранение диска. Только в личном OneDrive. |

### <a name="state-enumeration-values"></a>Значения государственного переумерия

| Значение      | Описание                                                                                                                                                                 |
| :--------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
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
