---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8ebca7ecd2ba49c3a14973bbc6060980c07927d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507459"
---
# <a name="contactfolder-resource-type"></a>Тип ресурса contactFolder

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Папка, содержащая контакты.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/contactfolder-delta.md).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение contactFolder](../api/contactfolder-get.md) | [contactFolder](contactfolder.md) |Получение папки с контактами с помощью идентификатора папки контактов.|
|[Обновление](../api/contactfolder-update.md) | [contactFolder](contactfolder.md) |Обновление объекта contactFolder. |
|[удаление](../api/contactfolder-delete.md); | Нет |Удаление объекта contactFolder. |
|[Список экземпляров childFolders](../api/contactfolder-list-childfolders.md) |Коллекция [contactFolder](contactfolder.md)| Получение коллекции дочерних папок для указанной папки с контактами.|
|[Создание дочернего элемента contactFolder](../api/contactfolder-post-childfolders.md) |[contactFolder](contactfolder.md)| Создание дочернего объекта contactFolder указанной папки.|
|[delta](../api/contact-delta.md)|Коллекция [contact](contact.md)| Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[Список контактов в папке](../api/contactfolder-list-contacts.md) |Коллекция [contact](contact.md)| Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.|
|[Создание контакта в папке](../api/contactfolder-post-contacts.md) |[contact](contact.md)| Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contactFolder](contactfolder.md)  |Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.   |
|[Получение contactFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contactFolder](contactfolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.  |
|[Получение contactFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Отображаемое имя папки.|
|id|String|Уникальный идентификатор папки с контактами. Только для чтения.|
|parentFolderId|String|Идентификатор родительской папки для папки.|
|wellKnownName|строка|Имя папки, если она является распознаваемой папкой. В `contacts` настоящее время это единственная распознанная папка контактов.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|childFolders|Коллекция [ContactFolder](contactfolder.md)|Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.|
|contacts|Коллекция [Contact](contact.md)|Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
