---
title: Получение Активитистатистикс
description: Получение свойств объекта Активитистатистикс для пользователя.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 9a85211faf15b6edbf843c5c604251dae06ae0a3
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450798"
---
# <a name="get-activitystatistics"></a>Получение Активитистатистикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств объекта [активитистатистикс](../resources/activitystatistics.md) для пользователя.

Можно получить свойства типа [активитистатистикс](../resources/activitystatistics.md) для указанного пользователя и диапазона дат. Вы можете указать тип статистики и диапазон дат, используя поддерживаемый формат для `id` [свойства идентификатора действия](../resources/activitystatistics.md#activity-id-property) в запросе.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Analytics. Read |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" }  -->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/{id}

GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}

```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный тип статистики действий, который является одним из следующих ресурсов, производных от [Активитистатистикс](../resources/activitystatistics.md): {[Call](../resources/callactivitystatistics.md), [Chat](../resources/chatactivitystatistics.md), [Email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), и [собрание](../resources/meetingactivitystatistics.md)}.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

В следующем примере запрашиваются статистические данные о типе Емаилактивитистатистикс пользователя, выполнившего вход в систему, в диапазоне дат от 2019-06-16 до 2019-06-17. Дополнительные сведения о формате свойства "общий идентификатор" можно узнать в разделе [свойство ID действия](../resources/activitystatistics.md#activity-id-property).

<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа, который получает статистику действий пользователя, выполнившего вход, для определенного действия и дня.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics/$entity",
    "@odata.type": "#microsoft.graph.emailActivityStatistics",
    "activity": "Email",
    "startDate": "2019-06-16",
    "endDate": "2019-06-17",
    "id": "email_2019-06-16_2019-06-17",
    "timeZoneUsed": "Pacific Standard Time",
    "duration": "PT0S",
    "afterHours": "PT0S",
    "readEmail": "PT0S",
    "sentEmail": "PT0S"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityStatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
