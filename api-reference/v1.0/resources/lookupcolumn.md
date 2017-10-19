---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: lookupColumn
ms.openlocfilehash: 07dba3c223ffc3993be1fc284572810a7aa3ccf8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="lookupcolumn-resource-type"></a>Тип ресурса lookupColumn

Ресурс **lookupColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.

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
| **allowMultipleValues**   | логический | Указывает, можно ли выбрать несколько значений в источнике.
| **allowUnlimitedLength**  | логический | Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.
| **columnName**            | строка  | Имя столбца-источника для подстановки.
| **listId**                | строка  | Уникальный идентификатор списка-источника для подстановки.
| **primaryLookupColumnId** | строка  | Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*. Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
