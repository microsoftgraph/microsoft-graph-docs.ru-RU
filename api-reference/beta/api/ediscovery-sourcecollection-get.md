---
title: Get sourceCollection
description: Ознакомьтесь с свойствами и отношениями объекта sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b10f29de6bbf61151f55aae2a37ac10ddf3ece86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446894"
---
# <a name="get-sourcecollection"></a>Get sourceCollection

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями [объекта sourceCollection.](../resources/ediscovery-sourcecollection.md)

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
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

Используйте для расширения операций набора `$expand` обзоров, источников хранителя и последней операции статистики оценки.

```http
https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и `200 OK` [объект microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.onmicrosoft.com"
        }
    },
    "addToReviewSetOperation": {
        "createdDateTime": "2021-01-13T05:38:49.9186654Z",
        "completedDateTime": "2021-01-13T07:54:45.0007868Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "addToReviewSet",
        "id": "aef586b34d89405d802497658a14194f",
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": null,
                "userPrincipalName": "admin@contoso.com"
            }
        }
    },
    "lastEstimateStatisticsOperation": {
        "createdDateTime": "2021-01-12T21:53:50.7272654Z",
        "completedDateTime": "2021-01-12T21:54:49.5595543Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "f3db0382af0842eaa98c7dd59e7dace6",
        "indexedItemCount": 39598,
        "indexedItemsSize": 3760920737,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 1,
        "siteCount": 1,
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": "EDisco Admin",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    }
}
```
