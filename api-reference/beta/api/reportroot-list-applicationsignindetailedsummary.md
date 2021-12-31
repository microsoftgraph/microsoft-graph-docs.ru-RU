---
title: List applicationSignInDetailedSummary
description: Получение объектов applicationSignInDetailedSummary.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 95c674d2ef36520b8a244c6c3ed78c38767acfa1
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647227"
---
# <a name="list-applicationsignindetailedsummary"></a>List applicationSignInDetailedSummary
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение [объектов applicationSignInDetailedSummary.](../resources/applicationsignindetailedsummary.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Reports.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/applicationSignInDetailedSummary
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$filter` `$top` запроса oData и OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_applicationsignindetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.applicationSignInDetailedSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#reports/applicationSignInDetailedSummary",
    "value": [
        {
            "id": "ce0d6f77-04d2-49f6-bfcc-ad101cd4b69f",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph Explorer",
            "aggregatedEventDateTime": "2021-12-28T00:00:00Z",
            "signInCount": 5,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            }
        },
        {
            "id": "59397b28-0dc5-4270-b869-24714ea4aedb",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph Explorer",
            "aggregatedEventDateTime": "2021-12-06T00:00:00Z",
            "signInCount": 5,
            "status": {
                "errorCode": 650057,
                "failureReason": "Invalid resource. The client has requested access to a resource which is not listed in the requested permissions in the client's application registration. Client app ID: {appId}({appName}). Resource value from request: {resource}. Resource app ID: {resourceAppId}. List of valid resources from app registration: {regList}.",
                "additionalDetails": null
            }
        },
        {
            "id": "29d5acee-e7c8-4565-96eb-f89719cb4d9f",
            "appId": "c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
            "appDisplayName": "Azure Portal",
            "aggregatedEventDateTime": "2021-12-28T00:00:00Z",
            "signInCount": 1,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            }
        },
        {
            "id": "88348b99-6c59-47db-bc70-2011d80e3bd6",
            "appId": "89bee1f7-5e6e-4d8a-9f3d-ecd601259da7",
            "appDisplayName": "Office365 Shell WCSS-Client",
            "aggregatedEventDateTime": "2021-11-30T00:00:00Z",
            "signInCount": 3,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            }
        }
    ]
}
```
