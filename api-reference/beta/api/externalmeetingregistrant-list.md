---
title: Список externalMeetingRegistrants
description: Получите список внешнихmeetingRegistrants onlineMeeting.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 81810e47432aaa0d64032ef481522620c02314a8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792024"
---
# <a name="list-externalmeetingregistrants"></a>Список externalMeetingRegistrants

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список [внешнихmeetingRegistrants](../resources/externalmeetingregistrant.md) [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetings.ReadWrite.All |

Чтобы использовать разрешение приложения для этого API, [](/graph/cloud-communication-online-meeting-application-access-policy) администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю для авторизации приложения, настроенного в политике, для получения онлайн-собраний и/или артефактов собраний в Интернете от имени этого пользователя (с пользовательским ИД, указанным в пути запроса).

## <a name="http-request"></a>HTTP-запрос

Чтобы получить список всех внешних регистраторов собраний с делегированной `/me` () и app `/users/{userId}/` () разрешения:

<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/registration/registrants
GET /users/{userId}/onlineMeetings/{meetingId}/registration/registrants
```

> [!TIP]
>
>- `userId`objectId  организатора собрания.
>- `meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов externalMeetingRegistrant](../resources/externalmeetingregistrant.md) в тексте ответа. Свойство **joinWebUrl** будет `null` .

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list-externalregistratrants"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
```

### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "list-externalregistratrants",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalMeetingRegistrant",
  "isCollection": true
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants",
  "value": [
    {
        "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
        "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
        "joinWebUrl": null,
        "userId": null,
        "tenantId": null
    },
    {
        "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
        "id": "e264916d-f65d-48ec-9c04-c2107fd5b61f",
        "joinWebUrl": null,
        "userId": null,
        "tenantId": null
    }
  ]
}
```
