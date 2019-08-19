---
title: Получение Активитистатистикс
description: Получение свойств объекта Активитистатистикс для пользователя.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d538b6389cd2a85768c15679d29d2fc9c11a0ff9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460810"
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


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
