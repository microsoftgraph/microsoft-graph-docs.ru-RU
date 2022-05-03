---
author: JeremyKelley
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.date: 09/11/2017
title: LookupColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d5ddc59f00b171d6ba7d125e8a626aa97ddcfff9
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176559"
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

| Свойство                  | Тип    | Описание                                                                                                                                                                                                                |
| :------------------------ | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **allowMultipleValues**   | boolean | Указывает, можно ли выбрать несколько значений в источнике.                                                                                                                                                         |
| **allowUnlimitedLength**  | boolean | Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.                                                                                                                      |
| **columnName**            | string  | Имя исходного столбца подстановки.                                                                                                                                                                                      |
| **listId**                | string  | Уникальный идентификатор исходного списка подстановки.                                                                                                                                                                           |
| **primaryLookupColumnId** | string  | Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*. Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца. |

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
