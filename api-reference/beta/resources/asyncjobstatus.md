---
author: JeremyKelley
description: Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 81348ce59e060dadf4201222fca43bf96241dbc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508173"
---
# <a name="asyncjobstatus-resource"></a>Ресурс AsyncJobStatus

Пространство имен: microsoft.graph

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
