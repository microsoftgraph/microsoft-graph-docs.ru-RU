---
author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Ниже показано представление ресурса ColumnDefinition в формате JSON.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4beefa8523898b4770de217a895426e9cc1f5cf91edbc6835b677d450ffc4943
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126671"
---
# <a name="columndefinition-resource"></a>Ресурс ColumnDefinition

Пространство имен: microsoft.graph

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса ColumnDefinition в формате JSON.

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

Ниже перечислены свойства ресурса **columnDefinition**.

| Имя свойства           | Тип    | Описание
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | строка  | Для столбцов сайтов это имя группы, к которой принадлежит данный столбец. Помогает упорядочивать связанные столбцы.
| **description**         | строка  | Описание столбца, которое видит пользователь.
| **displayName**         | строка  | Имя столбца, которое видит пользователь.
| **enforceUniqueValues** | логический | Если задано значение true, в соответствующем столбце не может быть нескольких элементов списка с одинаковыми значениями.
| **hidden**              | логический | Указывает, отображается ли столбец в пользовательском интерфейсе.
| **id**                  | строка  | Уникальный идентификатор столбца.
| **indexed**             | логический | Указывает, можно ли использовать значения столбцов для сортировки и поиска.
| **name**                | строка  | Используемое в API имя столбца из свойства [fields][] объекта [listItem][]. Имя, которое видит пользователь, указывается в свойстве **displayName**.
| **readOnly**            | логический    | Указывает, можно ли менять значения в столбце.
| **required**            | логический | Указывает, является ли значение в столбце обязательным.

В столбцах могут храниться данные различных типов.
Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.
Эти свойства являются взаимоисключающими. Для столбца можно указать только одно из них.

| Имя свойства     | Тип                    | Описание
|:------------------|:------------------------|:-------------------------------
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

Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.
Хотя наиболее распространенные типы полей представлены выше, этот API по-прежнему отсутствует некоторые из них.
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
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->