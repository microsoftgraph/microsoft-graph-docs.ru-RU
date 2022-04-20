---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: f51cea4ec7ca24c228ad7d4c92459f4c81cf3a45
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917782"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a>reportRoot: getTeamsDeviceUsageUserDetail

Пространство имен: microsoft.graph

Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

**Примечание**. Для делегированных разрешений, позволяющих приложениям считывать отчеты об использовании служб от имени пользователя, администратор клиента должен назначить пользователю соответствующую роль Azure Active Directory администратора. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date='{date_value}')
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения для {period_value}: `D7`, `D30`, и `D90``D180`. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. |
| date      | Date   | Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие. Значение {date_value} указывается в формате ГГГГ-ММ-ДД. Так как этот отчет доступен только за последние 28 дней, {date_value} должен быть датой из этого диапазона. |

> **Примечание:** Необходимо задать точку **или** дату **в** URL-адресе.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (Дата обновления отчета);
- Идентификатор пользователя
- "User Principal Name" (Имя участника-пользователя);
- Last Activity Date (Дата последнего действия);
- Is Deleted (Удален);
- Deleted Date (Дата удаления);
- Used Web (использовал браузер);
- Used Windows Phone (использовал телефон с Windows);
- Used iOS (использовал iOS);
- Used Mac (использовал Mac);
- Used Android Phone (использовал телефон с Android);
- Used Windows (использовал Windows);
- Report Period (Отчетный период).

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
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

Report Refresh Date,User Id,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
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

