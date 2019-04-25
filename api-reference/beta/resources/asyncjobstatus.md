---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544035"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
