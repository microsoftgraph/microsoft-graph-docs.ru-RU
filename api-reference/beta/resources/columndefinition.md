---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: ddd6b3c6d3048bf7a6d3ab2dbc8ff7259651ee2f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481162"
---
# <a name="columndefinition-resource-type"></a>Тип ресурса columnDefinition

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса columnDefinition в формате JSON.

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
  "enforceUniqueValues": "true",
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
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a>Свойства

В столбцах могут храниться данные различных типов.
Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.
Свойства, связанные с типами (Boolean, вычисляемые, Choice, Currency, dateTime, Lookup, Number, Персонорграуп, Text), являются взаимно исключающими — столбец может содержать только один из них.

| Имя свойства           | Тип    | Описание
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | строка  | Для столбцов сайтов это имя группы, к которой принадлежит данный столбец. Помогает упорядочивать связанные столбцы.
| **description**         | string  | Описание столбца, которое видит пользователь.
| **displayName**         | string  | Имя столбца, которое видит пользователь.
| **enforceUniqueValues** | логический | Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.
| **hidden**              | boolean | Указывает, отображается ли столбец в пользовательском интерфейсе.
| **id**                  | string  | Уникальный идентификатор столбца.
| **indexed**             | логический | Указывает, можно ли использовать значения столбцов для сортировки и поиска.
| **name**                | string  | Используемое в API имя столбца из свойства [fields][] объекта [listItem][]. Имя, которое видит пользователь, указывается в свойстве **displayName**.
| **readOnly**            | логический    | Указывает, можно ли менять значения в столбце.
| **required**            | логический | Указывает, является ли значение в столбце обязательным.
| **boolean**       | [booleanColumn][]       | В этом столбце хранятся логические значения.
| **calculated**    | [calculatedColumn][]    | Данные в этом столбце вычисляются относительно других столбцов.
| **choice**        | [choiceColumn][]        | В этом столбце хранятся данные из списка вариантов.
| **currency**      | [currencyColumn][]      | В этом столбце хранятся денежные значения.
| **dateTime**      | [dateTimeColumn][]      | В этом столбце хранятся значения даты и времени.
| **defaultValue**  | [defaultColumnValue][]  | Значение по умолчанию для этого столбца.
| **географическое положение**   | [Жеолокатионколумн][]   | В этом столбце хранится географическое положение.
| **lookup**        | [lookupColumn][]        | Данные в этом столбце берутся из другого источника на сайте.
| **number**        | [numberColumn][]        | В этом столбце хранятся числовые значения.
| **personOrGroup** | [personOrGroupColumn][] | В этом столбце хранятся значения людей или групп.
| **text**          | [textColumn][]          | В этом столбце хранятся текстовые значения.

>**Примечание:** Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.
Несмотря на то, что наиболее распространенные типы полей представлены в предыдущей таблице, этот API по-прежнему отсутствует.
При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.

## <a name="remarks"></a>Примечания

По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.
Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.
Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[Жеолокатионколумн]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": [
    "Error: /api-reference/beta/resources/columndefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
