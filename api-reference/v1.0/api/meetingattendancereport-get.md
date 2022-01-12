---
title: Get meetingAttendanceReport
description: Получите отчет о посещаемости для собрания в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: af9fa6e85082c7dbc16808e5852205cab6227af6
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861002"
---
# <a name="get-meetingattendancereport"></a>Get meetingAttendanceReport

Пространство имен: microsoft.graph

Получите [meetingAttendanceReport](../resources/meetingAttendanceReport.md) для [onlineMeeting](../resources/onlinemeeting.md). Каждый раз, когда собрание в Интернете заканчивается, для этого сеанса будет создан отчет о посещаемости.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetingArtifact.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application | OnlineMeetingArtifact.Read.All |

Чтобы использовать разрешение приложения для этого API, администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю. Это разрешает приложению, настроенное в политике, получать артефакты собраний и/или онлайн-собраний от имени этого пользователя (с ИД пользователя, указанного в пути запроса). Дополнительные сведения см. в материале [Разрешить приложениям получать](/graph/cloud-communication-online-meeting-application-access-policy)доступ к собраниям в Интернете от имени пользователя.

## <a name="http-request"></a>HTTP-запрос

Чтобы получить отчет о посещаемости по ID с делегированием `/me` () и приложением `/users/{userId}` () разрешения:

<!-- { "blockType": "ignored" } -->

```http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}
```

> [!TIP]
>
>- `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Дополнительные сведения см. в материале [Разрешить приложениям получать](/graph/cloud-communication-online-meeting-application-access-policy)доступ к собраниям в Интернете от имени пользователя.
>- `meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)
>- `reportId`— **это id** объекта [meetingAttendanceReport.](../resources/meetingAttendanceReport.md)

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

> [!TIP]
> Свойство **attendanceRecords** — это свойство навигации, которое не возвращается по умолчанию. Чтобы получить **в строке attendanceRecords,** используйте параметр `$expand=attendanceRecords` запроса, как показано в [примере.](#example)

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект meetingAttendanceReport](../resources/meetingAttendanceReport.md) в тексте ответа.

## <a name="example"></a>Пример

В следующем примере показано, как получить отчет о посещаемости для собрания в Интернете с делегированного разрешения.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get-attendanceReport-by-id"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/c9b6db1c-d5eb-427d-a5c0-20088d9b22d7?$expand=attendanceRecords
```

### <a name="response"></a>Отклик

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports('c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')",
  "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
  "totalParticipantCount": 1,
  "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
  "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
  "attendanceRecords": [
    {
      "emailAddress": "frederick.cormier@contoso.com",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4623",
        "displayName": "Frederick Cormier",
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
