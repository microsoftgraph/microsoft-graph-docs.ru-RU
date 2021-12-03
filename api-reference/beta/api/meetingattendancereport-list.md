---
title: List meetingAttendanceReports
description: Получите список отчетов о посещаемости для собрания в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4d575e06d0a672142264473a3a2fa9e2d79ff78e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285175"
---
# <a name="list-meetingattendancereports"></a>List meetingAttendanceReports

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [meetingAttendanceReport](../resources/meetingAttendanceReport.md) для [onlineMeeting.](../resources/onlinemeeting.md) Каждый раз, когда собрание в Интернете заканчивается, для этого сеанса создается отчет о посещаемости.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetingArtifact.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetingArtifact.Read.All |

Чтобы использовать разрешение приложения для этого API, администраторы клиентов должны создать [политику](/graph/cloud-communication-online-meeting-application-access-policy) доступа к приложениям и предоставить ее пользователю. Это разрешает приложению, настроенное в политике, получать артефакты собраний и/или онлайн-собраний от имени этого пользователя (с ИД пользователя, указанного в пути запроса).

## <a name="http-request"></a>HTTP-запрос

Чтобы получить все отчеты о посещаемости для онлайн-встречи с делегированной `/me` () и приложением `/users/{userId}` () разрешения:
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendanceReports
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports
```

> [!TIP]
>
>- `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)
>- `meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и список объектов `200 OK` [meetingAttendanceReport](../resources/meetingAttendanceReport.md) в тексте ответа.

> [!TIP]
> Свойство **attendanceRecords** пусто в ответе.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-attendanceReports"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendancereports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendancereports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendancereports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendancereports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-attendancereports-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "get-attendanceReports",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports",
  "value": [
    {
      "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
      "totalParticipantCount": 1,
      "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
      "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
      "attendanceRecords": []
    },
    {
      "id": "2c2c2454-7613-4d6e-9c7c-4cf7a6cdce89",
      "totalParticipantCount": 2,
      "meetingStartDateTime": "2021-10-04T23:13:31.658Z",
      "meetingEndDateTime": "2021-10-04T23:18:57.563Z",
      "attendanceRecords": []
    }
  ]
}
```
