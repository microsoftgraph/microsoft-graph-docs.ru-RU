---
title: 'accessReviewHistoryInstance: generateDownloadUri'
description: Создайте универсальный код ресурса (URI), который можно использовать для получения данных журнала проверки.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: af77906c4c5e978e6fc6a26fdfbe966b505f2c80
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696639"
---
# <a name="accessreviewhistoryinstance-generatedownloaduri"></a>accessReviewHistoryInstance: generateDownloadUri

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает URI для объекта [accessReviewHistoryInstance](../resources/accessReviewHistoryInstance.md)**, состояние** которого равно `done`. Каждый URI можно использовать для получения данных журнала проверки экземпляра. Каждый URI действителен в течение 24 часов и может быть получен путем получения свойства **downloadUri** из объекта [accessReviewHistoryInstance](../resources/accessReviewHistoryInstance.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.ReadWrite.All|

Чтобы создать ссылку, вошед в систему пользователь должен быть либо создателем связанного определения журнала проверки, либо назначен роль глобального  администратора или  [глобального читателя](/azure/active-directory/roles/permissions-reference).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identityGovernance/accessReviews/historyDefinitions/{accessReviewHistoryDefinitionId}/instances/{accessReviewHistoryInstanceId}/generateDownloadUri
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код `200 OK` отклика и [accessReviewHistoryInstances](../resources/accessReviewHistoryInstance.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewhistoryinstance_generatedownloaduri"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/instances/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewhistoryinstance-generatedownloaduri-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewhistoryinstance-generatedownloaduri-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewhistoryinstance-generatedownloaduri-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewhistoryinstance-generatedownloaduri-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewhistoryinstance-generatedownloaduri-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryInstance"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
    "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
    "reviewHistoryPeriodStartDateTime": "2000-06-19T08:00:00Z",
    "reviewHistoryPeriodEndDateTime": "2100-06-19T07:00:00Z",
    "status": "done",
    "runDateTime": "2022-01-20T17:46:54.6085806Z",
    "fulfilledDateTime": "2022-01-20T10:00:24.9114365-08:00",
    "downloadUri": "https://dfermconsolreportusc.blob.core.windows.net/df-erm-reports/Last months reviews for ELM-e642e792-9884-413d-9299-982b37bfe369.csv?skoid=fa04d013-9f36-4d7d-8b8e-7276fb3bd36e&sktid=33e01921-4d64-4f8c-a055-5bdaffd5e33d&skt=2022-01-20T18:03:59Z&ske=2022-01-20T18:05:59Z&sks=b&skv=2020-04-08&sv=2020-04-08&st=2022-01-20T18:04:01Z&se=2022-01-21T18:04:01Z&sr=b&sp=r&sig=...",
    "expiration": "2022-02-19T10:00:24.9114365-08:00"
}
```
