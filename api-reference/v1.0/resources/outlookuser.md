---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
ms.openlocfilehash: 63bbabccc540046961d31c91fe7b1fb9afaaf4f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027715"
---
# <a name="outlookuser-resource-type"></a>Тип ресурса outlookUser


Представляет службы Outlook, доступные пользователю.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Создание объекта **outlookCategory** в основном списке категорий пользователя.|
|[Перечисление категорий](../api/outlookuser-list-mastercategories.md) | Коллекция [outlookCategory](outlookcategory.md) |Получение всех категорий, определенных для пользователя.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Коллекция [localeInfo](localeinfo.md) | Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Коллекция [timeZoneInformation](timezoneinformation.md) | Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя. |


## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|masterCategories|Коллекция [outlookCategory](../resources/outlookcategory.md)| Список категорий, определенных для пользователя. | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->