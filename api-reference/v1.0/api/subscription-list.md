---
title: Перечисление подписок
description: Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 603a918faa9153f4b8690613a2b9aed7b7f53420
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273145"
---
# <a name="list-subscriptions"></a>Перечисление подписок

Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.

## <a name="permissions"></a>Разрешения

Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения  | Разрешения (в порядке повышения привилегий)  |
|:---------------- |:-------------------------------------------- |
| [Делегированное разрешение](/graph/auth-v2-user) (рабочая или учебная учетная запись) | Роль, необходимая для [создания подписки](subscription-post-subscriptions.md), или Subscription.Read.All (см. ниже). |
| [Делегированное разрешение](/graph/auth-v2-user) (личная учетная запись Майкрософт) | Роль, необходимая для [создания подписки](subscription-post-subscriptions.md), или Subscription.Read.All (см. ниже). |
| [Разрешение приложения](/graph/auth-v2-service) | Роль, необходимая для [создания подписки](subscription-post-subscriptions.md). |

Результаты отклика основаны на контексте приложения, отправившего вызов. Ниже представлена сводка общих сценариев.

### <a name="basic-scenarios"></a>Основные сценарии

Чаще всего приложению нужно получить подписки, изначально созданные им для текущего пользователя или для всех пользователей в каталоге (рабочих или учебных учетных записей). В этих сценариях не требуется никаких особых разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.

| Контекст приложения, отправившего вызов | Состав отклика |
|:-----|:---------------- |
| Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение). <br/>-и-<br/>У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям. | Подписки, созданные **этим приложением** только для вошедшего пользователя. |
| Приложение отправляет вызов от своего имени (разрешение приложения).<br/>-и-<br/>У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание. Это относится только к рабочим или учебным учетным записям.| Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.|

### <a name="advanced-scenarios"></a>Расширенные сценарии

В некоторых случаях приложению нужно получить подписки, созданные другими приложениями. Например, пользователь хочет просмотреть все подписки, созданные каким-либо приложением от его имени. Администратору может потребоваться просмотреть все подписки из всех приложений в своем каталоге.
В таких сценариях требуется делегированное разрешение Subscription.Read.All.

| Контекст приложения, отправившего вызов | Состав отклика |
|:-----|:---------------- |
| Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение). *Пользователь не является администратором*. <br/>-и-<br/>У приложения есть разрешение Subscription.Read.All<br/><br/>Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям. | Подписки, созданные **любым приложением** только для вошедшего пользователя. |
| Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение). *Пользователь является администратором*.<br/>-и-<br/>У приложения есть разрешение Subscription.Read.All<br/><br/>Примечание. Это относится только к рабочим или учебным учетным записям. | Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.|

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика.  Обратите внимание, что он может быть усечен для краткости.  При фактическом вызове будут возвращены все поддерживаемые свойства, соответствующие запросу и контексту вызова.

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
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
#### <a name="sdk-sample-code"></a>Образец кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscriptions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_subscriptions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.  Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).
