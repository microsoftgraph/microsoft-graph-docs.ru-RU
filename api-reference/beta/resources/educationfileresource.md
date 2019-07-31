---
title: Тип ресурса Едукатионфилересаурце
description: Подкласс Едукатионресаурце, представляющий объект File, связанный с назначением или отправкой.  В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе. Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 678591d4c9662f1ab3fc68f7d35a0ec525c6e74f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972746"
---
# <a name="educationfileresource-resource-type"></a>Тип ресурса Едукатионфилересаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс [едукатионресаурце](educationresource.md) , представляющий объект File, связанный с назначением или отправкой.  В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе. Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Расположение на диске файлового ресурса.|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
