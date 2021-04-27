---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Получение сведений об активных пользователях Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ebb4c09758fec323e015cf2efbda6b04f1e8cf5a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050908"
---
# <a name="reportroot-getoffice365activeuserdetail"></a>reportRoot: getOffice365ActiveUserDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение сведений об активных пользователях Microsoft 365.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a>Параметры функции

В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | string | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде. |
| date      | Date   | Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие. Значение {date_value} указывается в формате ГГГГ-ММ-ДД. Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона. |

> **Примечание.** В URL-адресе необходимо указать либо период, либо дату.

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа. Тип вывода по умолчанию — текст/csv. Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

### <a name="csv"></a>CSV

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (Дата обновления отчета);
- "User Principal Name" (Имя участника-пользователя);
- "Display Name" (Отображаемое имя);
- "Is Deleted" (Удалено);
- "Deleted Date" (Дата удаления);
- "Has Exchange License" (Есть лицензия на Exchange);
- "Has OneDrive License" (Есть лицензия на OneDrive);
- "Has SharePoint License" (Есть лицензия на SharePoint);
- "Has Skype For Business License" (Есть лицензия на Skype для бизнеса);
- "Has Yammer License" (Есть лицензия на Yammer);
- "Has Teams License" (Есть лицензия на Teams);
- "Exchange Last Activity Date" (Дата последнего действия в Exchange);
- "OneDrive Last Activity Date" (Дата последнего действия в OneDrive);
- "SharePoint Last Activity Date" (Дата последнего действия в SharePoint);
- "Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);
- "Yammer Last Activity Date" (Дата последнего действия в Yammer);
- "Teams Last Activity Date" (Дата последнего действия в Teams);
- "Exchange License Assign Date" (Дата назначения лицензии на Exchange);
- "OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);
- "SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);
- "Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);
- "Yammer License Assign Date" (Дата назначения лицензии на Yammer);
- "Teams License Assign Date" (Дата назначения лицензии на Teams);
- "Assigned Products" (Назначенные продукты).

Следующие столбцы не поддерживаются в Microsoft Graph Китае, выполняемых 21Vianet:

- "Has Yammer License" (Есть лицензия на Yammer);
- "Has Teams License" (Есть лицензия на Teams);
- "Yammer Last Activity Date" (Дата последнего действия в Yammer);
- "Teams Last Activity Date" (Дата последнего действия в Teams);
- "Yammer License Assign Date" (Дата назначения лицензии на Yammer);
- "Teams License Assign Date" (Дата назначения лицензии на Teams);

### <a name="json"></a>JSON

В случае успеха этот метод возвращает код отклика и `200 OK` **[объект Office365ActiveUserDetail](../resources/office365activeuserdetail.md)** в тексте ответа.

Следующие свойства объекта **[Office365ActiveUserDetail](../resources/office365activeuserdetail.md)** не поддерживаются в Microsoft Graph Китае под управлением 21Vianet:

- hasYammerLicense
- hasTeamsLicense
- yammerLastActivityDate
- teamsLastActivityDate
- yammerLicenseAssignDate
- teamsLicenseAssignDate

Размер страницы по умолчанию для этого запроса составляет 200 элементов.

## <a name="example"></a>Пример

### <a name="csv"></a>CSV

Ниже приводится пример, который выводит CSV.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a>JSON

Ниже приводится пример, который возвращает JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ]
    }
  ]
}
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


