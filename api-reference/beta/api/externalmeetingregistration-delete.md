---
title: Удаление externalMeetingRegistration
description: Отключить и удалить внешнюю регистрацию собрания.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6f9ca192567cf1b5d4073d4ed6810bc861f120e5
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565189"
---
# <a name="delete-externalmeetingregistration"></a>Удаление externalMeetingRegistration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отключить и удалить [внешнийMeetingRegistration](../resources/externalmeetingregistration.md) [onlineMeeting](../resources/onlinemeeting.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetings.ReadWrite.All |

Чтобы использовать разрешение приложения для этого API, [](/graph/cloud-communication-online-meeting-application-access-policy) администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю для авторизации приложения, настроенного в политике, для получения онлайн-собраний и/или артефактов собраний в Интернете от имени этого пользователя (с пользовательским ИД, указанным в пути запроса).

## <a name="http-request"></a>HTTP-запрос

Удаление регистрации внешних собраний с делегированием `/me` () и разрешением приложения `/users/{userId}/` () :

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}/registration
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration
```

> [!TIP]
>
>- `userId`objectId  организатора собрания.
>- `meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает только `204 No Content` код ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "delete-external-registration"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "delete-external-registration"
}-->

```http
HTTP/1.1 204 No Content
```
