---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
ms.openlocfilehash: 63bcf8f4084053356819601cd6306ad3ff5238c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836122"
---
# <a name="update-subscription"></a>Обновление подписки

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Возобновление подписки путем увеличения срока действия.

Срок действия подписок после продолжительность времени, зависит от типа ресурса. Во избежание отсутствует уведомлений, приложение следует обновлять его подписки еще до которых истек срок действия. В разделе [подписки](../resources/subscription.md) для Максимальная длина подписки для каждого типа ресурсов.

## <a name="permissions"></a>Разрешения

В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип ресурса или элемент        | Разрешение          |
|-----------------------------|---------------------|
| Contacts                    | Contacts.Read       |
| Беседы               | Group.Read.All      |
| События                      | Calendars.Read      |
| Сообщения                    | Mail.Read           |
| Группы                      | Group.Read.All      |
| Пользователи                       | User.Read.All       |
| Диск (хранилище OneDrive пользователя)    | Files.ReadWrite.     |
| На дисках (содержимое общих SharePoint и диски) | Files.ReadWrite.All |
|Предупреждение системы безопасности               | SecurityEvents.ReadWrite.All |

***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов. Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a>Ответ

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
