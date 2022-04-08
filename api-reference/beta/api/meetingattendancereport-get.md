---
title: Получение meetingAttendanceReport
description: Получение отчета об участии в собрании по сети.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 684e4cdd80c74c11d4118aa769bf15882d94ed4d
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704475"
---
# <a name="get-meetingattendancereport"></a>Получение meetingAttendanceReport

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите [meetingAttendanceReport](../resources/meetingAttendanceReport.md) для [onlineMeeting](../resources/onlinemeeting.md). Каждый раз, когда собрание по сети завершается, для этого сеанса создается отчет о присутствии.

> [!WARNING]
> Этот метод не поддерживает собрания каналов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetingArtifact.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | OnlineMeetingArtifact.Read.All |

Чтобы использовать разрешение приложения для этого API, администраторы клиента должны создать политику доступа к приложениям и предоставить ее пользователю. Это позволяет приложению, настроенное в политике, получать сетевые собрания и (или) артефакты собраний по сети от имени этого пользователя (с идентификатором пользователя, указанным в пути запроса). Дополнительные сведения см. в разделе "Разрешить приложениям доступ к собраниям по сети [от имени пользователя"](/graph/cloud-communication-online-meeting-application-access-policy).

## <a name="http-request"></a>HTTP-запрос

Чтобы получить отчет о присутствии по идентификатору с делегированным разрешением (`/me`) и разрешением приложения (`/users/{userId}`):
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}
```

Чтобы получить отчет об участии в последнем сеансе онлайн-собрания с делегированным (`/me`) и разрешением приложения (`/users/{userId}`) выполните указанные ниже действия.
<!-- { "blockType": "ignored" }-->
```http
GET /me/onlineMeetings/{meetingId}/meetingAttendanceReport
GET /users/{userId}/onlineMeetings/{meetingId}/meetingAttendanceReport
```

> [!TIP]
>
>- `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Дополнительные сведения см. в разделе "Разрешить приложениям доступ к собраниям по сети [от имени пользователя"](/graph/cloud-communication-online-meeting-application-access-policy).
>- `meetingId` — **это идентификатор** объекта [onlineMeeting](../resources/onlinemeeting.md) .
>- `reportId` — **это идентификатор** объекта [meetingAttendanceReport](../resources/meetingAttendanceReport.md) .

> [!CAUTION]
>
>- Путь `/meetingAttendanceReport` является устаревшим. В дальнейшем используйте путь для `/attendanceReports` получения отчетов об участии в собрании по сети.
>- Путь `/meetingAttendanceReport` останется в бета-версии для обеспечения обратной совместимости. Однако, чтобы получить тот же ответ, необходимо добавить параметр `expand` запроса. Дополнительные сведения см. в разделе ["Необязательные параметры запроса](#optional-query-parameters) ".

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

> [!TIP]
> Свойство **attendanceRecords** — это свойство навигации, которое не возвращается по умолчанию. Чтобы получить **attendanceRecords** в строке, используйте параметр `$expand=attendanceRecords` запроса, как показано в [примере 2](#example-2-get-the-latest-attendance-report-for-an-online-meeting).

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [meetingAttendanceReport](../resources/meetingAttendanceReport.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="example-1-get-the-attendance-report-for-an-online-meeting-by-id"></a>Пример 1. Получение отчета об участии в онлайн-собрании по идентификатору

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get-attendanceReport-by-id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/2c2c2454-7613-4d6e-9c7c-4cf7a6cdce89?$expand=attendanceRecords
```

#### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "get-attendanceReport-by-id",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports('c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')",
  "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
  "totalParticipantCount": 1,
  "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
  "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
  "attendanceRecords": [
    {
      "emailAddress": "(email address)",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-the-latest-attendance-report-for-an-online-meeting"></a>Пример 2. Получение последнего отчета об участии в собрании по сети

В следующем примере показан запрос на получение отчета об участии в собрании для последнего сеанса собрания по сети.

#### <a name="request"></a>Запрос

В следующем запросе используется делегированное разрешение.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attendance_report"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendance-report-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendance-report-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendance-report-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendance-report-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-attendance-report-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-attendancereport-by-id-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

В следующем запросе используется разрешение приложения.
<!-- { "blockType": "ignored" }-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```

#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport",
  "name": "get_attendance_report"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('dc74d9bb-6afe-433d-8eaa-e39d80d3a647')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')/meetingAttendanceReport/$entity",
  "attendanceRecords": [
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1558,
      "role": "Organizer",
      "identity": {
        "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:46.598956Z",
          "leaveDateTime": "2021-03-16T19:25:45.4473057Z",
          "durationInSeconds": 1558
        }
      ]
    },
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ],
  "totalParticipantCount": 2
}
```
