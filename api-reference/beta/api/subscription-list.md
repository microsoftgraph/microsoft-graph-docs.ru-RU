---
title: Список подписок
description: " сценарии ниже для получения дополнительных сведений см."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510983"
---
# <a name="list-subscriptions"></a>Список подписок

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка webhook подписки. Содержимое ответа зависит от контекста, в котором вызов приложения; сценарии ниже для получения дополнительных сведений см.

## <a name="permissions"></a>Разрешения

Этот интерфейс API поддерживает следующие области разрешений; [для получения дополнительных сведений, включая выбор разрешений, см.](/graph/permissions-reference)

| Тип разрешения  | Разрешения (в порядке повышения привилегий)  |
|:---------------- |:-------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись) | Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже). |
| Делегированные (личная учетная запись Майкрософт) | Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже). |
| [Application](/graph/auth-v2-service) | Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md). |

Результаты ответа зависят от контекста вызова приложения. Ниже приведен перечень распространенных сценариев:

### <a name="basic-scenarios"></a>Основные сценарии

Чаще всего приложения, где требуется реализовать для получения подписки, для которых он создан для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочего/школа учетные записи). Эти сценарии не требуются любые специальные разрешения, помимо тех, которые соответствуют приложения, изначально используется для создания его подписки.

| Контекст приложения, вызывающего | Содержит ответа |
|:-----|:---------------- |
| Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений). <br/>And<br/>Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей. | Подписки, созданные **в этом приложении** выполнил вход только для пользователя. |
| Приложение вызов от имени самого (разрешений приложения).<br/>And<br/>Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание: Это относится к рабочих/школа только для учетных записей.| Подписки, созданные **в этом приложении** для себя или для любого пользователя в каталоге.|

### <a name="advanced-scenarios"></a>Дополнительные сценарии

В некоторых случаях приложения, где требуется реализовать для получения подписки, созданные в других приложениях. Например пользователю для просмотра всех подписок, созданных любого приложения от их имени. Или администратор может потребоваться просмотреть все подписки из всех приложений в своих каталогов.
Для таких сценариев делегированных разрешений Subscription.Read.All является обязательным.

| Контекст приложения, вызывающего | Содержит ответа |
|:-----|:---------------- |
| Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений). *Пользователь является без прав администратора*. <br/>And<br/>Приложение имеет разрешение Subscription.Read.All<br/><br/>Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей. | Подписки, созданные в **любое приложение** выполнил вход только для пользователя. |
| Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений). *Пользователь является администратором*.<br/>And<br/>Приложение имеет разрешение Subscription.Read.All<br/><br/>Примечание: Это относится к рабочих/школа только для учетных записей. | Подписки, созданные с **любого приложения** для **любого пользователя** в каталоге.|

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [подписки](../resources/subscription.md) в теле ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a>Ответ

Ниже приведен пример отклика. Примечание: Для краткости может усекаться ответа, показано ниже. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

При возврате нескольких страниц данных ответа включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результаты.  Для получения дополнительных сведений см [Microsoft Graph постраничного просмотра данных в вашем приложении](/graph/paging).
