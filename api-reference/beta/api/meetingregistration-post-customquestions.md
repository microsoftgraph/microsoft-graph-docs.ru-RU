---
title: Создание meetingRegistrationQuestion
description: Создайте настраиваемый вопрос регистрации собраний, связанный с объектом meetingRegistration.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0dbbf42b3beaeb46538e2ea230a5e3a34892bb87
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61561505"
---
# <a name="create-meetingregistrationquestion"></a>Создание meetingRegistrationQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте [настраиваемый вопрос регистрации,](../resources/meetingregistrationquestion.md) связанный с объектом [meetingRegistration](../resources/meetingregistration.md) от имени организатора.

> [!TIP]
> При создании регистрации собраний можно создавать настраиваемые вопросы регистрации в строке. Дополнительные сведения см. [в материале Create meetingRegistration.](meetingRegistration-post.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | OnlineMeetings.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{id}/registration/microsoft.graph.meetingRegistration/customQuestions
```

> [!TIP]
> Чтобы получить `/customQuestions` доступ, следуйте [примеру,](#example) чтобы ввести тип **регистрации** **в meetingRegistration.**

## <a name="request-headers"></a>Заголовки запросов

| Имя            | Описание               |
| :-------------- | :------------------------ |
| Авторизация   | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В корпусе запроса поставляют представление JSON о writable свойствах объекта [meetingRegistrationQuestion.](../resources/meetingregistrationquestion.md)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект meetingRegistrationQuestion](../resources/meetingregistrationquestion.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create-custom-question"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/microsoft.graph.meetingRegistration/customQuestions
Content-Type: application/json

{
  "displayName": "What's your job position?",
  "isRequired": false,
  "answerInputType": "text"
}
```

### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "create-custom-question",
  "@odata.type": "microsoft.graph.meetingRegistrationQuestion"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/microsoft.graph.meetingRegistration/customQuestions/$entity",
  "id": "MSNhYjc5NWI4MC119zX3gwMDIwX3lvdXJfeDAwMjBfam8=",
  "displayName": "What's your job position?",
  "isRequired": false,
  "answerInputType": "text",
  "answerOptions": []
}
```
