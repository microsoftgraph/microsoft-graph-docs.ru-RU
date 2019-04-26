---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a649de502728bbc51ac53e072c08d95291d20853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568606"
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

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|masterCategories|Коллекция [outlookCategory](../resources/outlookcategory.md)| Список категорий, определенных для пользователя. | 
|Таскфолдерс|Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Папки задач Outlook пользователя. Только для чтения. Допускается значение null.|
|taskGroups|Коллекция [outlookTaskGroup](outlooktaskgroup.md)| Группы задач Outlook пользователя. Только для чтения. Допускается значение null.|
|tasks|Коллекция [outlookTask](outlooktask.md)| Задачи Outlook пользователя. Только для чтения. Допускается значение null.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
