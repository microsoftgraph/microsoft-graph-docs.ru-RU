---
author: JeremyKelley
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 813b31b61e3f510107cdd27ed64ec44fba9d0550
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522892"
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
