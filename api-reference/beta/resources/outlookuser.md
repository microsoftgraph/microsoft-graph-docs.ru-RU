---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bf772eb1598b38550797458df955495dafdd4282
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943601"
---
# <a name="outlookuser-resource-type"></a>Тип ресурса outlookUser

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет службы Outlook, доступные пользователю.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Создание объекта **outlookCategory** в основном списке категорий пользователя.|
|[Перечисление категорий](../api/outlookuser-list-mastercategories.md) | Коллекция [outlookCategory](outlookcategory.md) |Получение всех категорий, определенных для пользователя.|
|[Создание outlookTaskFolder](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.|
|[Список taskFolders](../api/outlookuser-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md) коллекции| Получите все папки задач Outlook в почтовом ящике пользователя.|
|[Создание outlookTaskGroup](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| Создайте группу задач Outlook в почтовом ящике пользователя.|
|[Список taskGroups](../api/outlookuser-list-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md) коллекции| Получение всех групп задач Outlook в почтовом ящике пользователя.|
|[Создание outlookTask](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| Создание задачи Outlook в группе задач по умолчанию (`My Tasks`) и папки задач по умолчанию (`Tasks`) в почтовом ящике пользователя.|
|[Перечисление задач](../api/outlookuser-list-tasks.md) |[outlookTask](outlooktask.md) коллекции| Получите все задачи Outlook в почтовом ящике пользователя.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Коллекция [localeInfo](localeinfo.md) | Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Коллекция [timeZoneInformation](timezoneinformation.md) | Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |


## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|masterCategories|Коллекция [outlookCategory](../resources/outlookcategory.md)| Список категорий, определенных для пользователя. | 
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md) коллекции| Папки задач Outlook пользователя. Только для чтения. Допускается значение null.|
|taskGroups|[outlookTaskGroup](outlooktaskgroup.md) коллекции| Группы задач пользователя Outlook. Только для чтения. Допускается значение null.|
|tasks|[outlookTask](outlooktask.md) коллекции| Задачи Outlook пользователя. Только для чтения. Допускается значение null.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
