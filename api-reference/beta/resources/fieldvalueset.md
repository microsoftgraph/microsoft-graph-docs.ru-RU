---
author: JeremyKelley
description: Представляет значения столбца в ресурсе listItem.
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: dab7c315174342f68c6fcb045e46d7da9d32f06a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972049"
---
# <a name="fieldvalueset-resource"></a>Ресурс fieldValueSet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет значения столбца в ресурсе [listItem](listitem.md).

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **fieldValueSet** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": []
}
-->
