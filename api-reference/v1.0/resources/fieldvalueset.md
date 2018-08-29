---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: fieldValueSet
ms.openlocfilehash: b0e3accc05ddf10328f8d27f8798f865e579e529
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266606"
---
# <a name="fieldvalueset-resource"></a>Ресурс fieldValueSet

Представляет значения столбца в ресурсе [listItem](listItem.md).

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **fieldValueSet** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
      "optionalProperties": ["Author", "AuthorLookupId", "Name", "Color", "Quantity" ],
       "baseType": "microsoft.graph.entity", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a>Свойства

Каждое отображаемое для пользователя поле в элементе **listItem** возвращается в виде пары имя-значение в объекте **fieldValueSet**.
В примере выше используется список, состоящий из четырех столбцов: **Author** (Автор), **Name** (Имя), **Color** (Цвет) и **Quantity** (Количество).

По умолчанию поля подстановки (например, поле `Author` выше) не возвращаются.
Вместо этого сервер возвращает поле LookupId (например, поле `AuthorLookupId` выше), ссылающееся на элемент listItem, являющийся целевым элементом в подстановке.
Имя поля LookupId представляет собой исходное имя поля, за которым следует текст `LookupId`.

В одном запросе можно запросить до 12 полей подстановки.
Сервер возвратит значения подстановки, если запрос содержит оператор `select`, в котором указаны необходимые вам поля.
Пример.

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

В одном запросе вы можете запросить до 12 полей подстановки, а также любое количество "обычных" полей.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
