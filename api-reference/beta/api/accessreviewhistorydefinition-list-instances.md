---
title: Экземпляры списка (из accessReviewHistoryDefinition)
description: Извлечение экземпляров определения истории проверки доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5283ae971621745251891afac1b4fbc6ba0de736
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62803949"
---
# <a name="list-instances-of-an-accessreviewhistorydefinition"></a>Экземпляры списка (из accessReviewHistoryDefinition)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Извлечение экземпляров](../resources/accessreviewhistoryinstance.md) определения истории [проверки доступа](../resources/accessreviewhistorydefinition.md), созданного за последние 30 дней.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|AccessReview.ReadWrite.All|

Если подписанный пользователь не является глобальным администратором или глобальным читателем, возвращаются только определения, созданные пользователем, вписав его.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identityGovernance/accessReviews/historyDefinitions/{accessReviewHistoryDefinitionId}/instances
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код отклика и коллекцию [объектов accessReviewHistoryInstance](../resources/accessreviewhistoryinstance.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewhistoryinstance"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/90e28cb7-4b9a-48f7-ba4e-a2756fda01b2/instances
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewhistoryinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewhistoryinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewhistoryinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewhistoryinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewhistoryinstance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewHistoryInstance)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessReviewInstances",
    "@odata.count": 1,
    "value": [
        {
            "id": "61a617dd-238f-4037-8fa5-d800e515f5bc",
            "status": "Done",
            "reviewHistoryPeriodStartDate": "2021-02-01T00:00:00Z",
            "reviewHistoryPeriodEndDate": "2021-03-01T00:00:00Z",
            "fulfilledDateTime": "2021-03-01T01:38:15.7998393Z",
            "downloadUri": "https://dfermconsolreportusc.blob.core.windows.net/df-erm-reports/Last quarter's reviews - via graph 2-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-03-01T19:39:38.0000000Z&se=2021-03-02T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D"
        }
    ]
}
```
