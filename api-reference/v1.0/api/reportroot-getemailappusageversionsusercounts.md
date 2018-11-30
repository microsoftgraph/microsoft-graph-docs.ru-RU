---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
ms.openlocfilehash: 730bae521523f51a3ab41c1d480439fd4bc4a305
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027160"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a>reportRoot: getEmailAppUsageVersionsUserCounts

Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :--------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                           |
| Для приложений                            | Reports.Read.All                         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Параметры функций

В URL-адресе запроса укажите следующий параметр и действительное значение.

| Параметр | Тип   | Описание                              |
| :-------- | :----- | :--------------------------------------- |
| period    | строка | Указывает отчетный период. Поддерживаемые значения {period_value}: D7, D30, D90 и D180. Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде. Обязательный. |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                              |
| :------------ | :--------------------------------------- |
| Авторизация | Bearer {токен}. Обязательный.                |
| If-None-Match | Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`. Необязательный параметр. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета. Этот URL-адрес можно найти в заголовке `Location` отклика.

URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.

CSV-файл содержит столбцы со следующими заголовками:

- Report Refresh Date (дата обновления отчета)
- Outlook 2016
- Outlook 2013
- Outlook 2010
- Outlook 2007
- Undetermined (не определено)
- Report Period (отчетный период)

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```

#### <a name="response"></a>Ответ

Ниже приведен пример ответа.

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

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```
