---
title: Получить статус educationSynchronizationProfile
description: Получите состояние определенного профиля синхронизации школьных данных в клиенте. В ответе указывается состояние синхронизации.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fef6a53f112f9c7f5922e9242761e5365e9f15a5
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574143"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a>Получить статус educationSynchronizationProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите состояние определенного профиля синхронизации [школьных данных](../resources/educationsynchronizationprofile.md) в клиенте. В ответе указывается состояние синхронизации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                       | Разрешения (в порядке повышения привилегий)                 |
| :------------------------------------ | :---------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)    | EduAdministration.Read, EduAdministration.ReadWrite         |
| Делегированная (личная учетная запись Майкрософт) | Не поддерживается.                                              |
| Приложение                           | EduAdministration.Read.All, EduAdministration.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) в тексте ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-status-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
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


