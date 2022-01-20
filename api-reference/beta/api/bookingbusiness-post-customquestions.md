---
title: Создание bookingCustomQuestion
description: Создайте новый объект bookingCustomQuestion.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f1b8ee38c527d8972ee38014a51f6f38cb3bd3b6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106904"
---
# <a name="create-bookingcustomquestion"></a>Создание bookingCustomQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект bookingCustomQuestion.](../resources/bookingcustomquestion.md)

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
}
-->

```http
POST /bookingBusinesses/{bookingBusinessesId}/customQuestions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса указать JSON-представление объекта [bookingCustomQuestion.](../resources/bookingcustomquestion.md)

При создании **bookingCustomQuestion** можно указать следующие свойства.

| Свойство        | Тип              | Описание                                                                                                         |
| :-------------- | :---------------- | :------------------------------------------------------------------------------------------------------------------ |
| answerInputType | answerInputType   | Ожидаемый тип ответа. Допустимые значения: `text`, `radioButton`, `unknownFutureValue`. Необязательное свойство.    |
| answerOptions   | Коллекция строк | Список возможных значений ответов. Необязательное свойство.                                                                     |
| displayName     | Строка            | Вопрос. Наследуется [от bookingNamedEntity](../resources/bookingnamedentity.md). Обязательный. |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект bookingCustomQuestion](../resources/bookingcustomquestion.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomquestion_from_"
}
-->

```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774
Content-Type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomquestion-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomquestion-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```
