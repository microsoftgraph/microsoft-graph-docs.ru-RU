---
title: Создание externalMeetingRegistration
description: Включить внешнюю регистрацию для собрания в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b78d560ef4f8e7e9dad37ffc86ccbe64d0b722f7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123568"
---
# <a name="create-externalmeetingregistration"></a>Создание externalMeetingRegistration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Включить регистрацию [для onlineMeeting с](../resources/onlinemeeting.md) помощью внешней системы регистрации. На собрании в Интернете может быть включена только одна регистрация.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetings.ReadWrite.All |

Чтобы использовать разрешение приложения для этого API, [](/graph/cloud-communication-online-meeting-application-access-policy) администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю для авторизации приложения, настроенного в политике, для получения онлайн-собраний и/или артефактов собраний в Интернете от имени этого пользователя (с пользовательским ИД, указанным в пути запроса).

## <a name="http-request"></a>HTTP-запрос

Создание регистрации внешних собраний с делегированием `/me` () и приложением `/users/{userId}/` () разрешения:

<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{meetingId}/registration
POST /users/{userId}/onlineMeetings/{meetingId}/registration
```

> [!TIP]
>
>- `userId`objectId  организатора собрания.
>- `meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса

В теле запроса поставляем представление JSON объекта [externalMeetingRegistration.](../resources/externalmeetingregistration.md)

> [!IMPORTANT]
> Необходимо предоставить свойство **@odata.type,** чтобы указать тип регистрации. Дополнительные сведения см. в следующем [примере](#example).

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект externalMeetingRegistration](../resources/externalmeetingregistration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-externalregistration",
  "@odata.type": "microsoft.graph.externalMeetingRegistration"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "allowedRegistrant": "everyone"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalregistration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalregistration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalregistration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalregistration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-externalregistration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "create-externalregistration",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalMeetingRegistration"
}-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "id": "f23714a3-a2f4-4b1d-96d2-bfe9097e7163",
  "allowedRegistrant": "everyone"
}
```
