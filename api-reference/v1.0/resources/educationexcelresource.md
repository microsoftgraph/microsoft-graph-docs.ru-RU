---
title: тип ресурсов educationExcelResource
description: Подкласс educationResource. Этот тип ресурса представляет собой Excel документа.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0e91d927e493a578a5a067e5a1caa1795a066940
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59099030"
---
# <a name="educationexcelresource-resource-type"></a>тип ресурсов educationExcelResource

Пространство имен: microsoft.graph

Подкласс [educationResource](educationresource.md). Этот тип ресурса представляет собой Excel документа.  
 
>**Примечание:** Файл Excel должен быть в папке ресурса, связанной с объектом назначения или отправки, к которому принадлежит этот ресурс.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|Строка|Указатель на объект Excel файла.|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


