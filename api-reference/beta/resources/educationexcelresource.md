---
title: Тип ресурса educationExcelResource
description: 'Подкласс educationResource. Этот тип ресурсов представляет документа в формате Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 11f28da1f2acaecbdd4f57abe8c6c8a03fbac0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982374"
---
# <a name="educationexcelresource-resource-type"></a>Тип ресурса educationExcelResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Подкласс [educationResource](educationresource.md). Этот тип ресурсов представляет документа в формате Excel.  
 
>**Примечание:** Файл Excel должен находиться в папку ресурсов, связанного с объектом назначения или отправки, к которой принадлежит ресурс.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|Строка|Указатель на объект файла Excel.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
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
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
