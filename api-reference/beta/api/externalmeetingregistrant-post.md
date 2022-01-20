---
title: Создание externalMeetingRegistrant
description: Регистрация внешнего регистратора собраний.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ebe3963a0b1c91058f3a677e09ef83e64c154eee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118928"
---
# <a name="create-externalmeetingregistrant"></a>Создание externalMeetingRegistrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Регистрация [externalMeetingRegistrant на](../resources/externalmeetingregistrant.md) собрании в Интернете с включенной [поддержкой externalMeetingRegistration.](../resources/externalmeetingregistration.md) Организатор собрания зачисляет кого-то, предоставляя уникальный **id** во внешней системе регистрации и получает уникальный **joinWebUrl** этого регистратора.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetings.ReadWrite.All |

Чтобы использовать разрешение приложения для этого API, [](/graph/cloud-communication-online-meeting-application-access-policy) администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю для авторизации приложения, настроенного в политике, для получения онлайн-собраний и/или артефактов собраний в Интернете от имени этого пользователя (с пользовательским ИД, указанным в пути запроса).

## <a name="http-request"></a>HTTP-запрос

Создание внешнего регистратора собраний с делегированием () и `/me` приложением `/users/{userId}/` () разрешения:

<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{meetingId}/registration/registrants
POST /users/{userId}/onlineMeetings/{meetingId}/registration/registrants
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

- Если значение разрешенного **свойстваRegistrant** объекта [externalMeetingRegistration](../resources/externalmeetingregistration.md) составляет , поставляем id из внешней системы регистрации, `organization` **tenantId** и **userId** регистранта в Azure Active Directory. 
- Если значение разрешенного **свойстваRegistrant** объекта [externalMeetingRegistration](../resources/externalmeetingregistration.md) имеет значение, поставляем только `everyone` **id** из внешней системы регистрации.

> [!IMPORTANT]
>
>- ID **из** внешней системы регистрации может быть любой формой строки.
>- Необходимо предоставить свойство **@odata.type,** чтобы указать тип регистратора. Дополнительные сведения см. в [следующих примерах.](#examples)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект externalMeetingRegistrant](../resources/externalmeetingregistrant.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-enroll-a-registrant-when-the-meeting-registration-has-allowedregistrant-set-to-everyone"></a>Пример 1. Регистрация регистратора, когда регистрация собраний позволила установитьRegistrant на "все"

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add-externalregistratrant-public"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "9d96988d-a66a-46ce-aad7-0b245615b297"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-externalregistratrant-public-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-externalregistratrant-public-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-externalregistratrant-public-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-externalregistratrant-public-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "add-externalregistratrant-public",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NjliNTYxNjktNzAwNi00OTlhLWFmMWEtMGZhY2JjZGM5NmEy%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%2216664f75-11dc-4870-bec6-38c1aaa81431%22%2c%22prid%22%3a%229d96988d-a66a-46ce-aad7-0b245615b297%22%2c%22isPublic%22%3atrue%7d",
  "userId": null,
  "tenantId": null
}
```

### <a name="example-2-enroll-a-registrant-when-the-meeting-registration-has-allowedregistrant-set-to-organization"></a>Пример 2. Регистрация регистратора, если регистрация собрания позволиларегистрации установить "организация"

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add-externalregistratrant-private"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde37",
  "userId": "cc515404-b55c-466e-b896-992c918ecc01"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-externalregistratrant-private-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-externalregistratrant-private-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-externalregistratrant-private-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-externalregistratrant-private-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "add-externalregistratrant-private",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NjliNTYxNjktNzAwNi00OTlhLWFmMWEtMGZhY2JjZGM5NmEy%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%2216664f75-11dc-4870-bec6-38c1aaa81431%22%2c%22prid%22%3a%2230494ab7-7338-4592-bfec-a4333be2a0a6%22%2c%22isPublic%22%3afalse%7d",
  "userId": "909c6581-5130-43e9-88f3-fcb3582cde37",
  "tenantId": "cc515404-b55c-466e-b896-992c918ecc01"
}
```
