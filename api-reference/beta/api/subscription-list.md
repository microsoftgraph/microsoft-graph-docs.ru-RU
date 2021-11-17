---
title: Перечисление подписок
description: " см. ниже сценарии."
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: eaab61771feca5c5e1f900295509da5460c1e52d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002078"
---
# <a name="list-subscriptions"></a>Перечисление подписок

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка подписки на веб-ок. Содержимое ответа зависит от контекста, в котором вызывается приложение; см. ниже сценарии.

## <a name="permissions"></a>Разрешения

Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения  | Разрешения (в порядке повышения привилегий)  |
|:---------------- |:-------------------------------------------- |
| [Делегированная](/graph/auth-v2-user) (работа или учетная запись школы) | Разрешение, необходимое [для создания подписки](subscription-post-subscriptions.md) или подписки.Read.All (см. ниже). |
| [Делегированная](/graph/auth-v2-user) (личная учетная запись Майкрософт) | Разрешение, необходимое [для создания подписки](subscription-post-subscriptions.md) или подписки.Read.All (см. ниже). |
| [Приложение](/graph/auth-v2-service) | Разрешение, необходимое [для создания подписки.](subscription-post-subscriptions.md) |

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

Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Показанный здесь ответ может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
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

> **Примечание.** Значение свойства `clientState` не возвращается в целях безопасности.  

Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.  Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).
