---
title: Перечисление ediscoveryCases
description: Получение списка дел обнаружения электронных данных
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 29c693647fefbdb1a67a1488f63a238442e35b9a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441902"
---
# <a name="list-ediscoverycases"></a>Перечисление ediscoveryCases
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [ediscoveryCase](../resources/security-ediscoverycase.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases
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

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию [объектов ediscoveryCase](../resources/security-ediscoverycase.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/ediscoveryCases
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-ediscoverycase-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-ediscoverycase-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryCase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases",
    "@odata.count": 22,
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2022-05-19T23:30:41.23Z",
            "status": "active",
            "closedDateTime": null,
            "externalId": "",
            "id": "60f86305-ac3e-408b-baa2-ea585dd8b0c0",
            "displayName": "My case 1",
            "createdDateTime": "2022-05-19T23:30:41.23Z",
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": "MOD Administrator"
                }
            },
            "closedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": ""
                }
            }
        },
        {
            "description": "",
            "lastModifiedDateTime": "2022-05-18T23:05:07.82Z",
            "status": "active",
            "closedDateTime": null,
            "externalId": "",
            "id": "7acdda75-3559-4f93-9827-cbd4c89db033",
            "displayName": "My case 2",
            "createdDateTime": "2022-05-18T23:05:07.82Z",
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": "MOD Administrator"
                }
            },
            "closedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": ""
                }
            }
        }
    ]
}
```

