---
author: JeremyKelley
description: Этот ресурс представляет элемент в SharePoint списка.
title: Ресурс listItem
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bfda041c473da6d5d98c7c6b076ba9be276cd486
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060677"
---
# <a name="listitem-resource"></a>Ресурс listItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элемент объекта [list][] в SharePoint.

Все элементы в библиотеке документов SharePoint могут быть представлены как ресурс **listItem** или [driveItem][].

Значения столбцов в списке доступны через словарь `fieldValueSet`.

## <a name="tasks-on-a-listitem"></a>Задачи для ресурса listItem

Ниже перечислены задачи, доступные для ресурсов **listItem**.
Все приведенные ниже примеры относятся к объекту **[list][]**, например `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.

| Стандартная задача                    | Метод HTTP                                  |
| :----------------------------- | :------------------------------------------- |
| [Получение][]                        | GET /items/{item-id}                         |
| [Получение значений столбцов][Получение]       | GET /items/{item-id}?expand=fields           |
| [Получение аналитики][]              | GET /items/{item-id}/analytics               |
| [Получение действий по интервалу][] | GET /items/{item-id}/getActivitiesByInterval |
| [Создание][]                     | POST /items                                  |
| [Удаление][]                     | DELETE /items/{item-id}                      |
| [Обновление][]                     | PATCH /items/{item-id}                       |
| [Обновление значений столбцов][Обновление] | PATCH /items/{item-id}/fields                |
| [createLink][CreateLink]       | POST /items/{itemId}/createLink              |
|[Перечисление documentSetVersions](../api/listitem-list-documentsetversions.md)| GET /items/{item-id}/documentSetVersions |
|[Создание documentSetVersion](../api/listitem-post-documentsetversions.md)| POST /items/{item-id}/documentSetVersions |
|[Восстановление documentSetVersion](../api/documentsetversion-restore.md)| POST /items/{item-id}/documentSetVersions/{documentSetVersion-id}/restore |

[Получение]: ../api/listitem-get.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Создание]: ../api/listitem-create.md
[Удаление]: ../api/listitem-delete.md
[Обновление]: ../api/listitem-update.md
[CreateLink]: ../api/listitem-createlink.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **listItem** в формате JSON.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "documentSetVersions": [{"@odata.type": "microsoft.graph.documentSetVersion"}],
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl&quot;: &quot;url"
}
```

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса **listItem**.

| Свойство    | Тип                | Описание                        |
| :---------- | :------------------ | :--------------------------------- |
| contentType | [contentTypeInfo][] | Тип контента для данного элемента списка. |

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание                                                              |
| :------------------- | :---------------- | :----------------------------------------------------------------------- |
| id                   | string            | Уникальный идентификатор элемента. Только для чтения.                            |
| name                 | string            | Имя или название элемента.                                            |
| createdBy            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.                         |
| createdDateTime      | DateTimeOffset    | Дата и время создания элемента. Только для чтения.                       |
| description          | строка            | Текст с описанием элемента.                                       |
| eTag                 | string            | ETag для элемента. Только для чтения.                                            |
| lastModifiedBy       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.                   |
| lastModifiedDateTime | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.                 |
| parentReference      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.                |
| sharepointIds        | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения. |
| webUrl               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.                    |

## <a name="relationships"></a>Связи

 Ниже перечислены связи ресурса **listItem** с другими ресурсами.

| Связь | Тип                           | Описание                                                                                        |
| :----------- | :----------------------------- | :------------------------------------------------------------------------------------------------- |
| activities   | Коллекция [itemActivity][]    | Список последних действий, выполненных с элементом.                                        |
| analytics    | Ресурс [itemAnalytics][]     | Аналитические данные о действиях просмотра, выполненных для элемента.|
|documentSetVersions|[Коллекция documentSetVersion](../resources/documentsetversion.md)| Сведения о версии набора документов, созданной пользователем.|
| driveItem    | [driveItem][]                  | Для библиотек документов связь **driveItem** предоставляет ресурс listItem как объект **[driveItem][]** |
| fields       | [fieldValueSet][]              | Значения столбцов, установленные для данного элемента списка.                                                   |
| versions     | Коллекция [listItemVersion][] | Список предыдущих версий элемента списка.                                                    |

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem&quot;: &quot;#"
  },
  "suppressions": []
}
-->
