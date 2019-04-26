---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 74ead4ca8e45c5baebe3ea74377ce102d9e2ee88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328652"
---
# <a name="asyncjobstatus-resource"></a>Ресурс AsyncJobStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.

Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.

* [Копирование элемента](../api/driveitem-copy.md)

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a>Свойства

| Имя свойства          | Тип   | Описание                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| **percentageComplete** | Double | Значение от 0 до 100, указывающее процент выполнения.                          |
| **status**             | Строка | Строковое значение, сопоставляемое с перечислением возможных значений состояния задания. |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
