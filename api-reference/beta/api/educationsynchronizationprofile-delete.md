---
title: Удаление educationSynchronizationProfile
description: Удаление профиля синхронизации школьных данных в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2cc7d03b406888022fc8bab935af2b5118357c0c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574288"
---
# <a name="delete-a-educationsynchronizationprofile"></a>Удаление educationSynchronizationProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление профиля [синхронизации школьных данных](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения |
|:-----------|:----------|
| Делегированное (рабочая или учебная учетная запись) | EduAdministration.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный.  |
|Делегированная (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `202 Accepted` ответа и не возвращает текст ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


