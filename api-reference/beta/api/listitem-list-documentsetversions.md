---
title: Перечисление documentSetVersions
description: Получение списка версий элемента набора документов в списке.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: d72e340a9804ecd5e71f86767066154613ab48fa
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447373"
---
# <a name="list-documentsetversions"></a>Перечисление documentSetVersions
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка версий [элемента набора](../resources/documentsetversion.md) документов в [списке](../resources/list.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Приложение| Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All, Sites.Selected|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{siteId}/lists/{listId}/items/{itemId}/documentSetVersions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [documentSetVersion](../resources/documentsetversion.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_documentsetversion"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/root/lists/Documents/items/1/documentSetVersions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-documentsetversion-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-documentsetversion-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-documentsetversion-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-documentsetversion-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-documentsetversion-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-documentsetversion-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "name": "list_documentsetversion",
  "truncated": true,
  "@odata.type": "microsoft.graph.documentSetVersion",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "id": "2",
            "lastModifiedDateTime": "2022-04-05T04:55:29Z",
            "comment": "v2",
            "createdDateTime": "2022-04-05T04:55:29Z",
            "shouldCaptureMinorVersion": false,
            "lastModifiedBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            },
            "items": [
                {
                    "itemId": "a5d83ae7-8c3e-4a2c-bc3e-8f276db857bf",
                    "versionId": "1.0"
                },
                {
                    "itemId": "62d40672-befe-4017-934b-06372fd96022",
                    "versionId": "1.0"
                }
            ],
            "createdBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            }
        },
        {
            "id": "1",
            "lastModifiedDateTime": "2022-04-05T04:53:42Z",
            "comment": "v1",
            "createdDateTime": "2022-04-05T04:53:42Z",
            "shouldCaptureMinorVersion": false,
            "lastModifiedBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            },
            "items": [
                {
                    "itemId": "a5d83ae7-8c3e-4a2c-bc3e-8f276db857bf",
                    "versionId": "1.0"
                }
            ],
            "createdBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            }
        }
    ]
}
```

