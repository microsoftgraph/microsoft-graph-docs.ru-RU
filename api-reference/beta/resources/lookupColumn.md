---
author: JeremyKelley
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 80f213de59ecd49ba03c60e5aa6eeea990e2eee8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089317"
---
# <a name="lookupcolumn-resource-type"></a>Тип ресурса lookupColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **lookupColumn** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства             | Тип    | Описание
|:--------------------------|:--------|:---------------------------------------
| **allowMultipleValues**   | boolean | Указывает, можно ли выбрать несколько значений в источнике.
| **allowUnlimitedLength**  | boolean | Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.
| **columnName**            | string  | Имя исходного столбца подстановки.
| **listId**                | string  | Уникальный идентификатор исходного списка подстановки.
| **primaryLookupColumnId** | string  | Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*. Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->


