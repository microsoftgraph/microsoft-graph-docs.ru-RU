---
title: Список customQuestions
description: Получите список пользовательских вопросов регистрации, связанных с объектом meetingRegistration.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 60cf4ddfa5ffa3bc4be497f777bce570abe6ce56
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369527"
---
# <a name="list-customquestions"></a>Список customQuestions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список пользовательских вопросов [регистрации,](../resources/meetingregistrationquestion.md) связанных с объектом [meetingRegistration](../resources/meetingregistration.md) от имени организатора.

> [!TIP]
> Вы также можете использовать операцию [Get meetingRegistration,](meetingregistration-get.md) чтобы получить настраиваемые вопросы регистрации.

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
GET /me/onlineMeetings/{id}/registration/customQuestions
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

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [meetingRegistrationQuestion](../resources/meetingregistrationquestion.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list-custom-questions"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions
```

### <a name="response"></a>Отклик

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "list-custom-questions",
  "@odata.type": "Collection(microsoft.graph.meetingRegistrationQuestion)"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/customQuestions",
  "value": [
    {
      "id": "MSMxY2E2ZmE3OS1hOTY3LTQ4ZX3lvdV94MDAyMF9hX3gwMDIwX2RldmU=",
      "displayName": "Are you a developer?",
      "isRequired": true,
      "answerInputType": "radioButton",
      "answerOptions": [
        "Yes",
        "No"
      ]
    },
    {
      "id": "MSM4YzZhMTkTQjV2hlcmVfeDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
      "displayName": "Where did you hear about us?",
      "isRequired": false,
      "answerInputType": "text",
      "answerOptions": []
    }
  ]
}
```
