---
title: Перечисление подписок
description: " в приведенных ниже сценариях представлены подробные сведения."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537092"
---
# <a name="list-subscriptions"></a>Перечисление подписок

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка подписок на веб-перехватчик. Содержимое ответа зависит от контекста, в котором приложение вызывается; в приведенных ниже сценариях представлены подробные сведения.

## <a name="permissions"></a>Разрешения

Этот API поддерживает следующие области разрешений; Дополнительные сведения, в том числе выбор разрешений, приведены в разделе [разрешения](/graph/permissions-reference).

| Тип разрешения  | Разрешения (в порядке повышения привилегий)  |
|:---------------- |:-------------------------------------------- |
| [Делегированный](/graph/auth-v2-user) (Рабочая или учебная учетная запись) | Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже). |
| [Делегированный](/graph/auth-v2-user) (личная учетная запись Майкрософт) | Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже). |
| [Приложение](/graph/auth-v2-service) | Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md). |

Результаты отКлика основываются на контексте вызывающего приложения. Ниже приведен краткий обзор типичных сценариев.

### <a name="basic-scenarios"></a>Основные сценарии

Чаще всего приложению требуется получить подписки, которые она создала для текущего пользователя, выполнившего вход в систему, или для всех пользователей в каталоге (рабочие и учебные учетные записи). Для этих сценариев не требуются специальные разрешения за пределами того приложения, которое использовалось изначально для создания своих подписок.

| Контекст вызывающего приложения | Ответ содержит |
|:-----|:---------------- |
| Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение). <br/>с<br/>У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание: это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям. | Подписки, созданные **этим приложением** только для пользователя, выполнившего вход. |
| Приложение вызывается от имени самого себя (разрешение приложения).<br/>с<br/>У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание: это относится только к учетным записям рабочих и учебных заведений.| Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.|

### <a name="advanced-scenarios"></a>Расширенные сценарии

В некоторых случаях приложению требуется получить подписки, созданные другими приложениями. Например, пользователю необходимо просмотреть все подписки, созданные любым приложением от их имени. Кроме того, администратор может просмотреть все подписки на все приложения в своем каталоге.
В таких случаях необходимо делегировать подПиску с разрешениями. Read. ALL.

| Контекст вызывающего приложения | Ответ содержит |
|:-----|:---------------- |
| Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение). *Пользователь не является администратором*. <br/>с<br/>Приложение имеет подПиску на разрешения. Read. ALL<br/><br/>Примечание: это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям. | Подписки, созданные **любым приложением** только для пользователя, выполнившего вход. |
| Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение). *Пользователь является администратором*.<br/>с<br/>Приложение имеет подПиску на разрешения. Read. ALL<br/><br/>Примечание: это относится только к учетным записям рабочих и учебных заведений. | Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.|

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

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [Subscription](../resources/subscription.md) в тексте отклика.

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

Ниже приведен пример отклика. Note: ответ, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

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

Если запрос возвращает несколько страниц данных, ответ включает `@odata.nextLink` свойство, помогающее управлять результатами.  Дополнительные сведения см в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging).
