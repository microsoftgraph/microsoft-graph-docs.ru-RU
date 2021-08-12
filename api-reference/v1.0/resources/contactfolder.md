---
title: Тип ресурса contactFolder
description: Папка, содержащая контакты.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2501a97d21026ffe9cba907729822c2c72b0912b6ebfc20cb6591637089a2960
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184923"
---
# <a name="contactfolder-resource-type"></a>Тип ресурса contactFolder

Пространство имен: microsoft.graph

Папка, содержащая контакты.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/contactfolder-delta.md).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение contactFolder](../api/contactfolder-get.md) | [contactFolder](contactfolder.md) |Получение папки с контактами с помощью идентификатора папки контактов.|
|[Обновление](../api/contactfolder-update.md) | [contactFolder](contactfolder.md) |Обновление объекта contactFolder. |
|[Удаление](../api/contactfolder-delete.md) | Нет |Удаление объекта contactFolder. |
|[Список экземпляров childFolders](../api/contactfolder-list-childfolders.md) |Коллекция [ContactFolder](contactfolder.md)| Получение коллекции дочерних папок для указанной папки с контактами.|
|[Создание дочернего элемента contactFolder](../api/contactfolder-post-childfolders.md) |[ContactFolder](contactfolder.md)| Создание дочернего элемента contactFolder для указанной папки.|
|[delta](../api/contact-delta.md)|Коллекция [contact](contact.md)| Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[Список контактов в папке](../api/contactfolder-list-contacts.md) |Коллекция [contact](contact.md)| Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.|
|[Создание контакта в папке](../api/contactfolder-post-contacts.md) |[Contact](contact.md)| Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.|
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contactFolder](contactfolder.md)  |Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.   |
|[Получение contactFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contactFolder](contactfolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.  |
|[Получение contactFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Отображаемое имя папки.|
|id|String|Уникальный идентификатор папки с контактами. Только для чтения.|
|parentFolderId|String|Идентификатор родительской папки для папки.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|childFolders|Коллекция [ContactFolder](contactfolder.md)|Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.|
|contacts|Коллекция [Contact](contact.md)|Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

