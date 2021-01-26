---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 1e2902ed070622fc7042e8d32ea98f9c7c571389
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981454"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a>reportRoot: getSkypeForBusinessActivityUserDetail

Пространство имен: microsoft.graph

Получите сведения о действиях пользователей в Skype для бизнеса.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Microsoft 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. |
| date      | Date   | Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие. Значение {date_value} указывается в формате ГГГГ-ММ-ДД. Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона. |

> **Примечание.** В URL-адресе необходимо указать либо период, либо дату.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                              |
| :------------ | :--------------------------------------- |
| Авторизация | Bearer {token}. Обязательный.                |
| If-None-Match | Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`. Необязательный параметр. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- "Report Refresh Date" (Дата обновления отчета);
- "User Principal Name" (Имя участника-пользователя);
- "Is Deleted" (Удалено);
- "Deleted Date" (Дата удаления);
- Last Activity Date (дата последнего действия)
- Total Peer-to-peer Session Count (общее количество одноранговых сеансов)
- Total Organized Conference Count (общее количество организованных конференций)
- Total Participated Conference Count (общее количество конференций с участием пользователя)
- Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)
- Organized Conference Last Activity Date (дата последнего действия в организованной конференции)
- Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)
- Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)
- Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)
- Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)
- Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)
- Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)
- Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)
- Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)
- Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)
- Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)
- Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)
- Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)
- Organized Conference Web Count (количество организованных веб-конференций)
- Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)
- Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)
- Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)
- Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)
- Paricipated Conference IM Count (количество конференций с участием пользователя и обменом мгновенными сообщениями)
- Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)
- Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)
- Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)
- Participated Conference Web Count (количество веб-конференций с участием пользователя)
- Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)
- Assigned Products (назначенные продукты)
- "Report Period" (Отчетный период).

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```


#### <a name="response"></a>Отклик

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

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
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

