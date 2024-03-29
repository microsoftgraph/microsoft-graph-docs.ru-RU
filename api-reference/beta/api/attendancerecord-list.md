---
title: Список посещаемостиRecords
description: Получите список объектов attendanceRecord и их свойств.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6cb1ab164f37ed08e8c941f75ea8b5b455dc5dc6
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63670616"
---
# <a name="list-attendancerecords"></a>Список посещаемостиRecords
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [attendanceRecord](../resources/attendancerecord.md) и их свойств.

> [!TIP]
> Более удобный способ получения записей о посещаемости — это соответствие их отчету о посещаемости с помощью параметра `expand` запроса. Пример и дополнительные сведения см. в материале [Get attendance report](meetingattendancereport-get.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetingArtifact.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetingArtifact.Read.All |

Чтобы использовать разрешение приложения для этого API, администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю. Это разрешает приложению, настроенное в политике, получать артефакты собраний и/или онлайн-собраний от имени этого пользователя (с ИД пользователя, указанного в пути запроса). Дополнительные сведения см. в материале [Разрешить приложениям получать](/graph/cloud-communication-online-meeting-application-access-policy) доступ к собраниям в Интернете от имени пользователя.

## <a name="http-request"></a>HTTP-запрос

Чтобы получить записи отчетов о посещаемости с делегированным (`/me`) и приложением (`/users/{userId}`) разрешением:
<!-- {"blockType": "ignored"}-->
``` http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords
```

>- `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Дополнительные сведения см. в материале [Разрешить приложениям получать](/graph/cloud-communication-online-meeting-application-access-policy) доступ к собраниям в Интернете от имени пользователя.
>- `meetingId` является **id** объекта [onlineMeeting](../resources/onlinemeeting.md) .
>- `reportId` — **это id** объекта [meetingAttendanceReport](../resources/meetingAttendanceReport.md) .

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и коллекцию объектов [attendanceRecord](../resources/attendancerecord.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_attendancerecord"
}
-->

``` http
GET https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-attendancerecord-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-attendancerecord-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-attendancerecord-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-attendancerecord-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-attendancerecord-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-attendancerecord-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attendanceRecord)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "emailAddress": "frederick.cormier@contoso.com",
      "totalAttendanceInSeconds": 322,
      "role": "Organizer",
      "registrantId": null,
      "identity": {
        "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4623",
        "displayName": "Frederick Cormier",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-10-05T04:38:27.6027225Z",
          "leaveDateTime": "2021-10-05T04:43:49.7702391Z",
          "durationInSeconds": 322
        }
      ]
    },
    {
      "emailAddress": "lisa.adkins@contoso.com",
      "totalAttendanceInSeconds": 314,
      "role": "Presenter",
      "registrantId": null,
      "identity": {
        "id": "57caaef9-5ed0-48d5-8862-e5abfa71b3e9",
        "displayName": "Lisa Adkins",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-10-04T23:13:43.3776519Z",
          "leaveDateTime": "2021-10-04T23:18:57.5639338Z",
          "durationInSeconds": 314
        }
      ]
    }
  ]
}
```
