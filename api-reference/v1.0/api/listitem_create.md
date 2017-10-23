---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "Создание записи в списке SharePoint"
ms.openlocfilehash: f4b2aebcd2bdc78cd6b8920b0690763c3b5f8ec2
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2017
---
# <a name="create-a-new-item-in-a-list"></a>Создание элемента в списке

Создание элемента [listItem][] в [списке][].

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a>Тело запроса

В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.

## <a name="example"></a>Пример

В примере ниже показано, как создать элемент списка общего назначения.

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

**Примечание.** Ответ усечен для наглядности. При фактическом вызове будут возвращены свойства, используемые по умолчанию.

[list]: ../resources/list.md
[listItem]: ../resources/listItem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
