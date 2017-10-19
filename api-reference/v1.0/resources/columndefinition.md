---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: e5942ddee4b505243cb64121862ce9e89e52d245
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="columndefinition-resource"></a>Ресурс ColumnDefinition

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса ColumnDefinition в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnDefinition",
       "keyProperty": "id", "optionalProperties": [ ] } -->

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
| **lookup**        | [lookupColumn][]        | Данные в этом столбце берутся из другого источника на сайте.
| **number**        | [numberColumn][]        | В этом столбце хранятся числовые значения.
| **personOrGroup** | [personOrGroupColumn][] | В этом столбце хранятся значения людей или групп.
| **text**          | [textColumn][]          | В этом столбце хранятся текстовые значения.

Примечание. Эти свойства соответствуют перечислению [SPFieldType][] в SharePoint.
Выше перечислены наиболее распространенные типы полей, но в бета-версии API по-прежнему не хватает некоторых типов.
При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.

## <a name="remarks"></a>Примечания

По умолчанию ресурсы ColumnDefinition и значения полей для столбцов `hidden` не отображаются.
Чтобы увидеть их при перечислении ресурсов **columnDefinition**, включите параметр `hidden` в оператор `$select`.
Чтобы увидеть их при отображении значений **field** в ресурсах [listItem][listItem], укажите имена нужных столбцов в операторе `$select`.

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
