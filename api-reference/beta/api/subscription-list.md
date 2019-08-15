---
title: Перечисление подписок
description: " в приведенных ниже сценариях представлены подробные сведения."
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 1b8b27feb5d8f261b39e2fa090d1e708394490ff
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409861"
---
# <a name="list-subscriptions"></a>Перечисление подписок

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка подписок на веб-перехватчик. Содержимое ответа зависит от контекста, в котором приложение вызывается; в приведенных ниже сценариях представлены подробные сведения.

## <a name="permissions"></a>Разрешения

Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения  | Разрешения (в порядке повышения привилегий)  |
|:---------------- |:-------------------------------------------- |
| [Делегированный](/graph/auth-v2-user) (Рабочая или учебная учетная запись) | Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже). |
| [Делегированный](/graph/auth-v2-user) (личная учетная запись Майкрософт) | Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже). |
| [Application](/graph/auth-v2-service) | Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md). |

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

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Ответ

Ниже приведен пример отклика. Note: ответ, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
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
  ]
}
-->

Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.  Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).
