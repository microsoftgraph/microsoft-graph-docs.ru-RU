---
title: Регистраторы списков
description: Получите список собранийРегистранты onlineMeeting.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8a221365b030412a4988f4b33fff859328924e42
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370386"
---
# <a name="list-registrants"></a>Регистраторы списков

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список [собранийРегистранты](../resources/meetingregistrant.md) [onlineMeeting](../resources/onlinemeeting.md) от имени организатора.

Этот метод можно использовать для получения отчета о регистрации для [веб-Microsoft Teams вебинара.](https://support.microsoft.com/en-us/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.Read, OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{id}/registration/registrants
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов meetingRegistrant](../resources/meetingRegistrant.md) в тексте ответа. Свойства **joinWebUrl** и **questionId** будут `null` .

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list-registratrants"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
```

### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "list-registratrants",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.meetingRegistrant)"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants",
  "value": [
    {
      "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,Cuzk8JP_iTTWqCOyVcalVA",
      "registrationDateTime": "2021-10-02T00:07:16.882602Z",
      "joinWebUrl": null,
      "firstName": "Frederick",
      "lastName": "Cormier",
      "email": "frederick.cormier@contoso.com",
      "status": "registered",
      "customQuestionAnswers": [
        {
          "questionId": null,
          "displayName": "Are you a developer?",
          "value": "Yes"
        },
        {
          "questionId": null,
          "displayName": "Where did you hear about us?",
          "value": "Company"
        }
      ]
    },
    {
      "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqzLnbHG_muA,b0ezc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,UwWARTlCT0dzO0jsuuq5EA",
      "registrationDateTime": "2021-10-02T00:08:49.1053222Z",
      "joinWebUrl": null,
      "firstName": "Lisa",
      "lastName": "Adkins",
      "email": "lisa.adkins@contoso.com",
      "status": "registered",
      "customQuestionAnswers": [
        {
          "questionId": null,
          "displayName": "Are you a developer?",
          "value": "No"
        },
        {
          "questionId": null,
          "displayName": "Where did you hear about us?",
          "value": ""
        }
      ]
    }
  ]
}
```
