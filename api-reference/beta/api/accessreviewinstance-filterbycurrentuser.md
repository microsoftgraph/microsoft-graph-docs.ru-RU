---
title: 'accessReviewInstance: filterByCurrentUser'
description: Возвращает все объекты accessReviewInstance для данного рецензента.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: db6de64071645fe97d5fffa4e3968ea63db5578e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031507"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a>accessReviewInstance: filterByCurrentUser
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возвращает все объекты [accessReviewInstance](../resources/accessreviewinstance.md) в заданном [accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) где пользователь вызовов является рецензентом на одном или более [объектах accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

>[!NOTE]
>Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance. Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$select` параметры `$filter` запроса `$orderBy` `$skip` OData и для настройки `$top` ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/filterByCurrentUser(on='reviewer')
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "7ca879f0-77ea-4386-b110-776dec898935",
            "startDateTime": "2021-04-20T00:45:51.627Z",
            "endDateTime": "2021-04-23T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "00ef5dba-4a32-48b3-b18a-57b244c0c4ba",
            "startDateTime": "2021-04-13T00:45:51.627Z",
            "endDateTime": "2021-04-16T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
