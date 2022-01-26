---
title: 'accessReviewHistoryInstance: generateDownloadUri'
description: Создание URI, который можно использовать для получения данных истории отзывов.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2b586e5925f34bd74f7dc2351a6b91fa102767fd
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226088"
---
# <a name="accessreviewhistoryinstance-generatedownloaduri"></a>accessReviewHistoryInstance: generateDownloadUri

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает URI для [объекта accessReviewHistoryInstance,](../resources/accessReviewHistoryInstance.md) состояние которого  `done` . Каждый URI можно использовать для получения данных истории отзывов экземпляра. Каждый URI действителен в течение 24 часов и может быть извлечен путем получения свойства **downloadUri** из [объекта accessReviewHistoryInstance.](../resources/accessReviewHistoryInstance.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложения|AccessReview.ReadWrite.All|

Чтобы создать ссылку, пользователь, подписав, должен быть либо создателем связанного  определения  истории отзывов, либо назначены роли глобального администратора или глобального [каталога читателей.](/azure/active-directory/roles/permissions-reference)

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

В случае успеха это действие возвращает код отклика и `200 OK` [accessReviewHistoryInstances](../resources/accessReviewHistoryInstance.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "accessreviewhistoryinstance_generatedownloaduri"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/instances/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri
```

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
