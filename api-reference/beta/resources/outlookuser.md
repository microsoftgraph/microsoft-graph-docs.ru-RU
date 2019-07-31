---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2c23cccabcea33b8cdaacba6ae9abede456c5c99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009267"
---
# <a name="outlookuser-resource-type"></a>Тип ресурса outlookUser

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет службы Outlook, доступные пользователю.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Создание объекта **outlookCategory** в основном списке категорий пользователя.|
|[Перечисление категорий](../api/outlookuser-list-mastercategories.md) | Коллекция [outlookCategory](outlookcategory.md) |Получение всех категорий, определенных для пользователя.|
|[Создание outlookTaskFolder](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.|
|[Список Таскфолдерс](../api/outlookuser-list-taskfolders.md) |Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Получение всех папок задач Outlook в почтовом ящике пользователя.|
|[Создание outlookTaskGroup](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| Создайте группу задач Outlook в почтовом ящике пользователя.|
|[Список taskGroups](../api/outlookuser-list-taskgroups.md) |Коллекция [outlookTaskGroup](outlooktaskgroup.md)| Получение всех групп задач Outlook в почтовом ящике пользователя.|
|[Создание outlookTask](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.|
|[Перечисление задач](../api/outlookuser-list-tasks.md) |Коллекция [outlookTask](outlooktask.md)| Получение всех задач Outlook в почтовом ящике пользователя.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Коллекция [localeInfo](localeinfo.md) | Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Коллекция [timeZoneInformation](timezoneinformation.md) | Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |


## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|masterCategories|Коллекция [outlookCategory](../resources/outlookcategory.md)| Список категорий, определенных для пользователя. | 
|Таскфолдерс|Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Папки задач Outlook пользователя. Только для чтения. Допускается значение null.|
|taskGroups|Коллекция [outlookTaskGroup](outlooktaskgroup.md)| Группы задач Outlook пользователя. Только для чтения. Допускается значение null.|
|tasks|Коллекция [outlookTask](outlooktask.md)| Задачи Outlook пользователя. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
