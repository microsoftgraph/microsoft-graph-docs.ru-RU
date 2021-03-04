---
author: JeremyKelley
description: Вот представление JSON ресурса columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: aab34ebe8a0cb7539775ba3e7b07e8ad7b3c357b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444341"
---
# <a name="columndefinition-resource-type"></a>тип ресурса columnDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса columnDefinition.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": true,
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a>Свойства

В столбцах могут храниться данные различных типов.
Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.
Свойства типа (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) являются взаимоисключающими : столбец может иметь только один из указанных.

| Имя свойства           | Тип    | Описание
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | строка  | Для столбцов сайтов это имя группы, к которой принадлежит данный столбец. Помогает упорядочивать связанные столбцы.
| **description**         | string  | Описание столбца, которое видит пользователь.
| **displayName**         | string  | Имя столбца, которое видит пользователь.
| **enforceUniqueValues** | Boolean | Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.
| **hidden**              | Boolean | Указывает, отображается ли столбец в пользовательском интерфейсе.
| **id**                  | string  | Уникальный идентификатор столбца.
| **indexed**             | Boolean | Указывает, можно ли использовать значения столбцов для сортировки и поиска.
| **name**                | string  | Используемое в API имя столбца из свойства [fields][] объекта [listItem][]. Имя, которое видит пользователь, указывается в свойстве **displayName**.
| **readOnly**            | Boolean    | Указывает, можно ли менять значения в столбце.
| **required**            | Boolean | Указывает, является ли значение в столбце обязательным.
| **boolean**       | [booleanColumn][]       | В этом столбце хранятся логические значения.
| **calculated**    | [calculatedColumn][]    | Данные в этом столбце вычисляются относительно других столбцов.
| **choice**        | [choiceColumn][]        | В этом столбце хранятся данные из списка вариантов.
| **currency**      | [currencyColumn][]      | В этом столбце хранятся денежные значения.
| **dateTime**      | [dateTimeColumn][]      | В этом столбце хранятся значения даты и времени.
| **defaultValue**  | [defaultColumnValue][]  | Значение по умолчанию для этого столбца.
| **геолокация**   | [geolocationColumn][]   | В этом столбце хранится геолокация.
| **lookup**        | [lookupColumn][]        | Данные в этом столбце берутся из другого источника на сайте.
| **number**        | [numberColumn][]        | В этом столбце хранятся числовые значения.
| **personOrGroup** | [personOrGroupColumn][] | В этом столбце хранятся значения людей или групп.
| **text**          | [textColumn][]          | В этом столбце хранятся текстовые значения.
| **isDeletable**       | Boolean | Указывает, можно ли удалить этот столбец.
| **propagateChanges**     | Boolean | Если изменения "True" в этом столбце будут распространяться в списки, реализующих столбец. 
| **isReorderable**         | Boolean | Указывает, можно ли переуказать значения в столбце. Только для чтения.
| **isSealed**              | Boolean | Указывает, можно ли изменить столбец.
| **проверка**   |  [columnValidation][]    | В этом столбце хранится формула проверки и сообщение для столбца. 
| **hyperlinkOrPicture**  | [hyperlinkOrPictureColumn][] | В этом столбце хранится гиперссылка или значения изображения. 
| **термин**     | [termColumn][] | В этом столбце хранится таксономия терминов.
| **sourceContentType**   |[contentTypeInfo][]  | ContentType, от которого наследуется этот столбец. Используется только при извлечении столбцов contentTypes.
| **thumbnail**           |[thumbnailColumn][]      | В этом столбце хранится эскизные значения.
| **тип**         | columnTypes  | Для столбцов сайта тип столбца. Только для чтения
| **contentApprovalStatus**| [contentApprovalStatusColumn][]     | В этом столбце сохраняется состояние утверждения контента.

## <a name="relationships"></a>Связи

| Имя свойства   | Тип                      | Описание
|:----------------|:--------------------------|:-------------------------------
| **sourceColumn** | [columnDefinition][] | Столбец исходный для столбца типа контента.

>**Примечание:** Эти свойства соответствуют переумериям [SPFieldType в SharePoint.][]
Хотя наиболее распространенные типы полей представлены в предыдущей таблице, этот API бета-версии по-прежнему отсутствует.
При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.

## <a name="remarks"></a>Примечания

По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.
Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.
Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md

[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->