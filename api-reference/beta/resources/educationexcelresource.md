---
title: Тип ресурса Едукатионексцелресаурце
description: 'Подкласс объекта Едукатионресаурце. Этот тип ресурса представляет документ Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: be9ea1d08575ad9dc07ac9fe538a597da8db2803
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334429"
---
# <a name="educationexcelresource-resource-type"></a>Тип ресурса Едукатионексцелресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс объекта [едукатионресаурце](educationresource.md). Этот тип ресурса представляет документ Excel.  
 
>**Примечание:** Файл Excel должен находиться в папке ресурсов, связанной с назначением или объектом отправки, к которому принадлежит ресурс.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Указатель на объект файла Excel.|

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
