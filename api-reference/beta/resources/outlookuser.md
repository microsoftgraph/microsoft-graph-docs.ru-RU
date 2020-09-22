---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6473a7a3808982467f50bafc810cbca80e4ce0dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998343"
---
# <a name="outlookuser-resource-type"></a>Тип ресурса outlookUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Представляет службы Outlook, доступные пользователю.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Создание объекта **outlookCategory** в основном списке категорий пользователя.|
|[Перечисление категорий](../api/outlookuser-list-mastercategories.md) | Коллекция [outlookCategory](outlookcategory.md) |Получение всех категорий, определенных для пользователя.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Коллекция [localeInfo](localeinfo.md) | Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Коллекция [timeZoneInformation](timezoneinformation.md) | Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |
|[Создание outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (устаревшее) |[outlookTaskFolder](outlooktaskfolder.md)| Создайте папку задач в группе задач по умолчанию ( `My Tasks` ) почтового ящика пользователя.|
|[Список таскфолдерс](../api/outlookuser-list-taskfolders.md) (не рекомендуется) |Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Получение всех папок задач Outlook в почтовом ящике пользователя.|
|[Создание outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (устаревшее) |[outlookTaskGroup](outlooktaskgroup.md)| Создайте группу задач Outlook в почтовом ящике пользователя.|
|[Список taskGroups](../api/outlookuser-list-taskgroups.md) (не рекомендуется) |Коллекция [outlookTaskGroup](outlooktaskgroup.md)| Получение всех групп задач Outlook в почтовом ящике пользователя.|
|[Создание outlookTask](../api/outlookuser-post-tasks.md) (устаревшее) |[outlookTask](outlooktask.md)| Создайте задачу Outlook в группе задач по умолчанию ( `My Tasks` ) и папке задач по умолчанию ( `Tasks` ) в почтовом ящике пользователя.|
|[Список задач](../api/outlookuser-list-tasks.md) (не рекомендуется) |Коллекция объектов [outlookTask](outlooktask.md)| Получение всех задач Outlook в почтовом ящике пользователя.|



## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|masterCategories|Коллекция [outlookCategory](../resources/outlookcategory.md)| Список категорий, определенных для пользователя. | 
|Таскфолдерс (устаревший)|Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Папки задач Outlook пользователя. Только для чтения. Допускается значение null.|
|taskGroups (устаревший)|Коллекция [outlookTaskGroup](outlooktaskgroup.md)| Группы задач Outlook пользователя. Только для чтения. Допускается значение null.|
|задачи (не рекомендуется)|Коллекция объектов [outlookTask](outlooktask.md)| Задачи Outlook пользователя. Только для чтения. Допускается значение null.|

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


