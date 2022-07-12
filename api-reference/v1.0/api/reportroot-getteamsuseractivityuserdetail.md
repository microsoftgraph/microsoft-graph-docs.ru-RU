---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведений о действиях отдельных пользователей Microsoft Teams.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 934206863b13e5e7e3a1a5918f6fc630561fa470
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730387"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a>reportRoot: getTeamsUserActivityUserDetail

Пространство имен: microsoft.graph

Получение сведения о действиях отдельных пользователей Microsoft Teams.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

>**Примечание**. Чтобы делегированные разрешения позволяли приложениям читать отчеты об использовании службы от имени пользователя, администратор клиента должен назначить пользователю соответствующую роль администратора Azure AD с ограниченными правами. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. |
| date      | Date   | Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие. Значение {date_value} указывается в формате ГГГГ-ММ-ДД. Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона. |

> **Примечание.** В URL-адресе необходимо указать либо период, либо дату.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (Дата обновления отчета);
- Tenant Display Name (Отображаемое имя клиента);
- Shared Channel Tenant Display Names (Отображаемые имена клиентов общего канала);
- Идентификатор пользователя
- "User Principal Name" (Имя участника-пользователя);
- Last Activity Date (Дата последнего действия);
- Is Deleted (Удален);
- Deleted Date (Дата удаления);
- Assigned Products (Назначенные продукты);
- Team Chat Messages Count (Количество сообщений в чатах групп);
- Private Chat Message Count (Количество сообщений в приватных чатах);
- Call Count (Количество звонков);
- Meeting Count (Количество собраний);
- Post Messages (Публикация сообщений);
- Reply Messages (Ответные сообщения);
- Urgent Messages (Срочные сообщения);
- Meetings Organized Count (Количество организованных собраний);
- Meetings Attended Count (Количество посещенных собраний);
- Ad Hoc Meetings Organized Count (Количество организованных незапланированных собраний);
- Ad Hoc Meetings Attended Count (Количество посещенных незапланированных собраний);
- Scheduled One-time Meetings Organized Count (Количество организованных запланированных разовых собраний);
- Scheduled One-time Meetings Attended Count (Количество посещенных запланированных разовых собраний);
- Scheduled Recurring Meetings Organized Count (Количество организованных запланированных повторяющихся собраний);
- Scheduled Recurring Meetings Attended Count (Количество посещенных запланированных повторяющихся собраний);
- Audio Duration (Длительность аудио);
- Video Duration (Длительность видео);
- Screen Share Duration (Длительность демонстрации экрана);
- Audio Duration In Seconds (Длительность аудио в секундах);
- Video Duration In Seconds (Длительность видео в секундах);
- Screen Share Duration In Seconds (Длительность демонстрации экрана в секундах);
- Has Other Action (Есть другое действие);
- Is Licensed (Наличие лицензии);
- "Report Period" (Отчетный период).

> [!NOTE] 
> Значения в счетчике организованных совещаний могут не совпадать с суммой счетчика организованных разовых собраний, счетчика организованных запланированных разовых собраний и счетчика запланированных повторяющихся собраний, организованных пользователем в течение указанного периода времени. Это связано с тем, что значение "Неклассифицированные собрания" не включается в выходной CSV-файл. Подробнее см. в [отчете об активности пользователей Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-analytics-and-reports/user-activity-report).

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Tenant Display Name,Shared Channel Tenant Display Names,User Id,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Post Messages,Reply Messages,Urgent Messages,Meetings Organized Count,Meetings Attended Count,Ad Hoc Meetings Organized Count,Ad Hoc Meetings Attended Count,Scheduled One-time Meetings Organized Count,Scheduled One-time Meetings Attended Count,Scheduled Recurring Meetings Organized Count,Scheduled Recurring Meetings Attended Count,Audio Duration,Video Duration,Screen Share Duration,Audio Duration In Seconds,Video Duration In Seconds,Screen Share Duration In Seconds,Has Other Action,Is Licensed,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

