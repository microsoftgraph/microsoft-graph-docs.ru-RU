---
title: Создание meetingRegistrant
description: Регистрация регистратора собраний.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 00fe202935a202b68da020a82c306a087dae340e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980893"
---
# <a name="create-meetingregistrant"></a>Создание meetingRegistrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Зарегистрив [регистратор собрания,](../resources/meetingregistrant.md) [](../resources/meetingregistration.md) зарегистрив его, на собрании в Интернете с включенной регистрацией собраний от имени регистратора. Эта операция имеет два сценария:

- Если значение разрешенного **свойстваRegistrant** объекта [meetingRegistration](../resources/meetingregistration.md) имеет значение, регистраторы должны будут войти перед регистрацией `organization` на собрание. **FirstName**, **lastName** и **email** должны соответствовать сведениям, хранимым в Azure Active Directory (Azure AD).
- Если значение разрешенного **свойстваRegistrant** объекта [meetingRegistration](../resources/meetingregistration.md) является, регистраторы не должны будут войдывать и будут `everyone` считаться анонимными.

В любом случае регистратор получает уведомление по электронной почте с сведениями о регистрации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | OnlineMeetings.Read.All |

> [!TIP]
>
> - Если значение разрешенного **свойстваRegistrant** объекта [meetingRegistration](../resources/meetingregistration.md) является, используйте делегированное разрешение регистратора `organization` для регистрации.
> - Если значение разрешенного **свойстваRegistrant** объекта [meetingRegistration](../resources/meetingregistration.md) является, используйте делегированное разрешение регистратора `everyone` для регистрации.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/{id}/registration/registrants
```

> **Примечание:** `userId` является **объектомid** организатора собрания.

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В органе запроса поставляем представление JSON для редактируемых свойств объекта [meetingRegistrant.](../resources/meetingRegistrant.md)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и частичный `200 OK` [объект meetingRegistrant](../resources/meetingRegistrant.md) в тексте ответа.

> [!TIP]
> Тело ответа будет содержать различные сведения в зависимости от значения **allowedRegistrant**.
>
> - Если значение разрешенного **свойстваRegistrant** , только `organization` **id** и **joinWebUrl** будут возвращены в [объект meetingRegistrant.](../resources/meetingRegistrant.md) Регистраторы могут использовать **id,** чтобы отменить регистрацию или **присоединиться к Собранию.**
> - Если значение разрешенного **свойстваRegistrant** имеет значение, будет возвращен пустой объект `everyone` [meetingRegistrant.](../resources/meetingRegistrant.md) Регистраторы должны использовать ссылки в электронной почте, которые они получают, чтобы отменить регистрацию или присоединиться к собранию.

## <a name="examples"></a>Примеры

### <a name="example-1-enroll-a-signed-in-registrant"></a>Пример 1. Регистрация зарегистрированного регистратора

В следующем примере показано, как зарегистрировать зарегистрированного регистранта с делегированной разрешением регистратора, если собрание разрешило **наборуRegistrant** `organization` .

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add-registratrant-user"
}-->

```http
POST https://graph.microsoft.com/beta/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "firstName": "Frederick",
  "lastName": "Cormier",
  "email": "frederick.cormier@contoso.com",
  "customQuestionAnswers": [
    {
      "questionId": "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
      "value": "No"
    },
    {
      "questionId": "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
      "value": "Internet"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-registratrant-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-registratrant-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-registratrant-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-registratrant-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-registratrant-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "add-registratrant-user",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,E4jbleVFdE6BDf6ei3YBOA,KvXQzK4zfU-5LQj_ZLWgow,A7_SArco00S-Qr707l0vBA,UFakyZrk1K9vBacExW1muA",
  "registrationDateTime": null,
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MmE4Mzg1OTItYjg2Ni00ZmNmLWI5NjMtODNkZDJiMWNlNTVi%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5131-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%2c%22prid%22%3a%22gWWckDBR6UOI8_yzWCzeNw%2c6pAAiSa1bkGqzLnbHG_muA%2cbzLh6uR-5EGdsCvtvIvs6Q%2cE4jbleVFdE6BDf6ei3YBOA%2cKvXQzK4zfU-5LQj_ZLWgow%2cA7_SArco00S-Qr707l0vBA%2cUFaiyZrk1K9vBacExW1muA%22%2c%22isPublic%22%3afalse%7d",
  "firstName": null,
  "lastName": null,
  "email": null,
  "status": null,
  "customQuestionAnswers": []
}
```

### <a name="example-2-enroll-an-anonymous-registrant"></a>Пример 2. Регистрация анонимного регистратора

В следующем примере показано, как зарегистрировать анонимный регистратор с разрешения приложения, если собрание **разрешилорегистрации** установить `everyone` .

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add-registratrant-app"
}-->

```http
POST https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "firstName": "Lisa",
  "lastName": "Adkins",
  "email": "lisa.adkins@contoso.com",
  "customQuestionAnswers": [
    {
      "questionId": "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
      "value": "No"
    },
    {
      "questionId": "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
      "value": "Internet"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-registratrant-app-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-registratrant-app-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-registratrant-app-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-registratrant-app-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-registratrant-app-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "add-registratrant-app",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
    "id": "",
    "registrationDateTime": null,
    "joinWebUrl": "",
    "firstName": null,
    "lastName": null,
    "email": null,
    "status": null,
    "customQuestionAnswers": []
}
```
