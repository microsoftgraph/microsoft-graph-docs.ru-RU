---
title: 'sourceCollection: estimateStatistics'
description: Выполняет оценку коллекции исходных данных.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8935ff163e82f154420ca9acae247c164ea7554c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340265"
---
# <a name="sourcecollection-estimatestatistics"></a>sourceCollection: estimateStatistics

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запустите оценку количества электронных писем и документов в коллекции исходных данных. Дополнительные сведения о исходных коллекциях (также известных как поиски в eDiscovery) см. в примере Сбор данных для [случая в Advanced eDiscovery](/microsoft-365/compliance/collecting-data-for-ediscovery).

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
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

Если оценка успешно запущена, это действие возвращает код `202 Accepted` ответа. В ответе также будет содержаться `Location` заглавный загот, содержащий расположение [оценкиStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) , созданной для обработки оценки. Проверьте состояние операции оценки, сделав запрос GET в расположение, после успешного завершения [состояние изменится на](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollection_estimatestatistics"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollection-estimatestatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollection-estimatestatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollection-estimatestatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollection-estimatestatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/sourcecollection-estimatestatistics-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/sourcecollection-estimatestatistics-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: private
client-request-id: af32de50-99d9-e3a8-371b-a4f366cc78e7
content-length: 0
content-type: text/plain
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/82edd40e182a464fa02c24a36fa94873
request-id: e890176f-640f-4222-9cd8-be26e71c5e5d
```
