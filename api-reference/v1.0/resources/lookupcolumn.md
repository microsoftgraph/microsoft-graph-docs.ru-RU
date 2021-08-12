---
author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a619323598f3e648341ba533371f9a9c56026ab7ffa6196313aaaec13e39c74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149760"
---
# <a name="lookupcolumn-resource-type"></a>Тип ресурса lookupColumn

Пространство имен: microsoft.graph

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->

