---
title: 'приложение: setVerifiedPublisher'
description: Установка проверенного издателя приложения.
ms.localizationpriority: medium
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: bae85faa7adc5fb2152bb68a0f0e2a7864baf129
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982861"
---
# <a name="application-setverifiedpublisher"></a>приложение: setVerifiedPublisher

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Установите [проверенныйPublisher](../resources/verifiedPublisher.md) в [приложении.](../resources/application.md) Дополнительные сведения, включая необходимые условия для установки проверенного издателя, см. в Publisher [проверки.](/azure/active-directory/develop/publisher-verification-overview)

## <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
|Для приложений | Не поддерживается |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи следующие необходимые свойства.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| verifiedPublisherId | Строка | ID microsoft Partner Network (MPNID) проверенного издателя, который будет задат в приложении, из учетной записи Центра партнеров издателя. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_setverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/setVerifiedPublisher
Content-type: application/json

{
    "verifiedPublisherId": "1234567"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-setverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-setverifiedpublisher-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-setverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-setverifiedpublisher-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/application-setverifiedpublisher-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: e7beba93-bb0b-42ea-96c8-231aa61d755e
2020-09-09 21:16:07 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
