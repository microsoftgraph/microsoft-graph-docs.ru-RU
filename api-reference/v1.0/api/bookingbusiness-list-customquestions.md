---
title: Список customQuestions
description: Получите ресурсы bookingCustomQuestion, связанные с bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: aeac18a40b718724e3d7e7ab3516096024d204f9
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014252"
---
# <a name="list-customquestions"></a>Список customQuestions

Пространство имен: microsoft.graph

Получите ресурсы [bookingCustomQuestion,](../resources/bookingcustomquestion.md) связанные с [bookingBusiness.](../resources/bookingbusiness.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                    |
| :------------------------------------- | :----------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                 |
| Для приложений                            | Не поддерживается.                                                                 |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}-->

```http
GET /solutions/bookingBusinesses/{bookingBusinessesId}/customQuestions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в $count и $expand [параметров запроса OData.](/graph/query-parameters)

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [bookingCustomQuestion](../resources/bookingcustomquestion.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions
```

### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "isCollection": true
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.bookingCustomQuestion",
        "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
        "displayName": "What is your age?",
        "answerInputType": "text",
        "answerOptions": [],
    },
    {
        "@odata.type": "#microsoft.graph.bookingCustomQuestion",
        "id": "dbb865a6-530d-46e1-8e88-5d76789034b2",
        "displayName": "What is your nationality?",
        "answerInputType": "radioButton",
        "answerOptions": [
          "US",
          "UK",
          "Canada",
          "India"
        ],
    }
  ]
}
```
