---
author: JeremyKelley
description: Представляет столбец на сайте, списке или типе контента.
ms.date: 09/11/2017
title: тип ресурса columnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 05357e3282dfe578ed6756ddff493df9e62c8248
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695107"
---
# <a name="columndefinition-resource-type"></a>тип ресурса columnDefinition

Пространство имен: microsoft.graph


Представляет столбец на [сайте,][] [списке][]или [contentType.][]


СтолбцыDefinitions и значения поля для `hidden` столбцов не показаны по умолчанию.
Чтобы перечислить **скрытые столбцыDefinitions,** `hidden` включите в свое `$select` заявление.
Чтобы перечислить **скрытые** значения поля [в listItems][listItem,]включите нужные столбцы по имени в вашем `$select` заявлении.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список столбцов на сайте](../api/site-list-columns.md)|[коллекция columnDefinition](../resources/columndefinition.md)|Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств на [сайте.](../resources/site.md)|
|[Список столбцов в списке](../api/list-list-columns.md)|[коллекция columnDefinition](../resources/columndefinition.md)|Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств в [списке.](../resources/list.md)|
|[Список столбцов в типе контента](../api/contenttype-list-columns.md)|[коллекция columnDefinition](../resources/columndefinition.md)|Получите список объектов [columnDefinition](../resources/columndefinition.md) и их свойств в [типе контента.](../resources/contenttype.md)|
|[Создание columnDefinition для сайта](../api/site-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Создание нового [объекта columnDefinition](../resources/columndefinition.md) на [сайте.](../resources/site.md)|
|[Создание columnDefinition для списка](../api/list-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Создайте новый [объект columnDefinition](../resources/columndefinition.md) в [списке](../resources/list.md).|
|[Создание columnDefinition для типа контента](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Создание нового [объекта columnDefinition](../resources/columndefinition.md) в [типе контента.](../resources/contenttype.md)|
|[Получить columnDefinition](../api/columndefinition-get.md)|[columnDefinition](../resources/columndefinition.md)|Ознакомьтесь с свойствами и отношениями объекта [columnDefinition.](../resources/columndefinition.md)|
|[Обновление столбцаDefinition](../api/columndefinition-update.md)|[columnDefinition](../resources/columndefinition.md)|Обновление свойств объекта [columnDefinition.](../resources/columndefinition.md)|
|[Удаление columnDefinition](../api/columndefinition-delete.md)|Нет|Удаляет объект [columnDefinition.](../resources/columndefinition.md)|

## <a name="properties"></a>Свойства

В столбцах могут храниться данные различных типов.
Перечисленные ниже свойства указывают тип данных, которые хранятся в столбце, а также дополнительные параметры этих данных.
Свойства, связанные с типом (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text, term, hyperlinkOrPicture, thumbnail и contentApprovalStatus) являются взаимоисключающими; в столбце может быть указан только один из них.

| Имя свойства           | Тип    | Описание|
|:------------------------|:--------|:-----------------------------------------|
| **columnGroup**         | строка  | Для столбцов сайтов это имя группы, к которой принадлежит данный столбец. Помогает упорядочивать связанные столбцы.|
| **description**         | string  | Описание столбца, которое видит пользователь.|
| **displayName**         | string  | Имя столбца, которое видит пользователь.|
| **enforceUniqueValues** | Логический | Если для этого столбца нет двух элементов `true` списка, то для этого столбца может быть одинаковое значение.|
| **hidden**              | Boolean | Указывает, отображается ли столбец в пользовательском интерфейсе.|
| **id**                  | string  | Уникальный идентификатор столбца.|
| **indexed**             | Логический | Указывает, можно ли использовать значения столбца для сортировки и поиска.|
| **name**                | string  | Используемое в API имя столбца из свойства [fields][] объекта [listItem][]. Имя, которое видит пользователь, указывается в свойстве **displayName**.|
| **readOnly**            | Логический    | Указывает, можно ли менять значения в столбце.|
| **required**            | Логический | Указывает, является ли значение столбца необязательным.|
| **boolean**       | [booleanColumn][]       | В этом столбце хранятся логические значения.|
| **calculated**    | [calculatedColumn][]    | Данные в этом столбце вычисляются относительно других столбцов.|
| **choice**        | [choiceColumn][]        | В этом столбце хранятся данные из списка вариантов.|
| **currency**      | [currencyColumn][]      | В этом столбце хранятся денежные значения.|
| **dateTime**      | [dateTimeColumn][]      | В этом столбце хранятся значения даты и времени.|
| **defaultValue**  | [defaultColumnValue][]  | Значение по умолчанию для этого столбца.|
| **геолокация**   | [geolocationColumn][]   | В этом столбце хранится геолокация.|
| **lookup**        | [lookupColumn][]        | Данные в этом столбце берутся из другого источника на сайте.|
| **number**        | [numberColumn][]        | В этом столбце хранятся числовые значения.|
| **personOrGroup** | [personOrGroupColumn][] | В этом столбце хранятся значения людей или групп.|
| **text**          | [textColumn][]          | В этом столбце хранятся текстовые значения.|
| **isDeletable**       | Логический | Указывает, можно ли удалить этот столбец.|
| **propagateChanges**     | Логический | Если "true", изменения в этом столбце будут распространяться в списки, реализующих столбец. |
| **isReorderable**         | Логический | Указывает, можно ли переуказать значения в столбце. Только для чтения.|
| **isSealed**              | Логический | Указывает, можно ли изменить столбец.|
| **проверка**   |  [columnValidation][]    | В этом столбце хранится формула проверки и сообщение для столбца.| 
| **hyperlinkOrPicture**  | [hyperlinkOrPictureColumn][] | В этом столбце хранится гиперссылка или значения изображения. |
| **термин**     | [termColumn][] | В этом столбце хранится таксономия терминов.|
| **sourceContentType**   |[contentTypeInfo][]  | ContentType, от которого наследуется этот столбец. Присутствует только в столбцах contentTypes. Только для чтения.|
| **thumbnail**           |[thumbnailColumn][]      | В этом столбце хранится эскизные значения.|
| **type**         | columnTypes  | Для столбцов сайта тип столбца. Только для чтения.|
| **contentApprovalStatus**| [contentApprovalStatusColumn][]     | В этом столбце сохраняется состояние утверждения контента.|

## <a name="relationships"></a>Связи

| Имя свойства   | Тип                      | Описание|
|:----------------|:--------------------------|:-------------------------------|
| **sourceColumn** | [columnDefinition][] | Столбец исходный для столбца типа контента.|

>**Примечание:** Эти свойства соответствуют SharePoint [SPFieldType.][]
Обратите внимание, что наиболее распространенные типы полей представлены в предыдущей таблице. Однако этот API по-прежнему отсутствует.
При использовании этих типов не заполняются никакие аспекты типа столбца, а сам столбец обладает только основными свойствами.
Сайты и столбцы списков ответ не будет содержать **isDeletable,** **propagateChanges**, **isReorderable**, **isSealed**, проверка  **,**  **hyperlinkOrPicture** **,** термин , **sourceContentType** **,** эскиз , **тип**, **contentApprovalStatus** и **sourceColumn** свойства.

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

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[list]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[site]: site.md
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