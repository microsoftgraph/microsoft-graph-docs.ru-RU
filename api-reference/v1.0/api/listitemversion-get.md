---
title: Получение ресурса ListItemVersion
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса ListItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3e45cf260a9f526a7309c63791ed2cb6b8196e45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541397"
---
# <a name="get-a-listitemversion-resource"></a>Получение ресурса ListItemVersion

В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|            Тип разрешения             | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Sites.Read.All, Sites.ReadWrite.All         |
| Делегированные (личная учетная запись Майкрософт) | Н/д                                         |
| Для приложений                            | Sites.Read.All, Sites.ReadWrite.All         |


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.


## <a name="example"></a>Пример

В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a>Отклик

Возвращается коллекция версий:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
