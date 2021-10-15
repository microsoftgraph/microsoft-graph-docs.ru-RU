---
title: Удаление meetingRegistrant
description: Отмена регистрации onlineMeeting для собранияRegistrant.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5529c31b6b5bb0df1b51cb62f808ff7f389e07b4
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369497"
---
# <a name="unenroll-meeting-registrant"></a>Регистратор собраний unenroll

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отмена [регистрации onlineMeeting](../resources/onlinemeeting.md) для [собранияRegistrant](../resources/meetingregistrant.md) от имени регистратора.

Используйте этот метод только в том случае, если разрешенное **свойствоRegistrant** объекта [meetingRegistration](../resources/meetingregistration.md) имеет значение и для регистрации использовалось делегированное разрешение `organization` регистратора. Если **допустимо значениеRegistrant,** регистраторы могут использовать ссылку только в получаемом сообщении электронной почты, чтобы `everyone` отменить регистрацию.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetings.Read.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration/registrants/{id}
```

>**Примечания:**
>
> - `userId` является объектомid организатора собрания.
> - `meetingId`является **id** объекта [onlineMeeting.](../resources/onlineMeeting.md)

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает только `204 No Content` код ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "delete-registratrant-user"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants/gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,Cuzk8JP_iTTWqCOyVcalVA
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "name": "delete-registratrant-user",
}-->

```http
HTTP/1.1 204 No Content
```
