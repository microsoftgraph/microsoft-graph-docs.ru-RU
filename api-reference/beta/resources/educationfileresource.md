---
title: Тип ресурса educationFileResource
description: Подкласс educationResource, которая представляет собой объект-файл, который связан с назначения или отправки.  В этом случае файл не относится к одному из специальных файлов (Word, Excel и т. д.), но представляет собой файл, для которого не специальная обработка в системе. Файл ресурсов должно храниться в **resourceFolder** , который связан с назначения или отправки, которым связан этот ресурс.
localization_priority: Normal
ms.openlocfilehash: 5fda86b80030a2bc0c885b4dd90a384b7ede7fff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858088"
---
# <a name="educationfileresource-resource-type"></a>Тип ресурса educationFileResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Подкласс [educationResource](educationresource.md) , которая представляет собой объект-файл, который связан с назначения или отправки.  В этом случае файл не относится к одному из специальных файлов (Word, Excel и т. д.), но представляет собой файл, для которого не специальная обработка в системе. Файл ресурсов должно храниться в **resourceFolder** , который связан с назначения или отправки, которым связан этот ресурс.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|Строка|Место на диске файл ресурсов.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
