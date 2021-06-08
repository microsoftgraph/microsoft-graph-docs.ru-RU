---
title: Начните синхронизациюJob
description: Запустите существующее задание синхронизации. Если задание находится в приостановленной работе, она будет продолжать обработку изменений с точки, где она была приостановлена. Если задание находится на карантине, состояние карантина будет очищено.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 510722b4571abec22bfda27aee117033391268b8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787183"
---
# <a name="start-synchronizationjob"></a>Начните синхронизациюJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запустите существующее задание синхронизации. Если задание находится в приостановленной работе, она будет продолжать обработку изменений с точки, где она была приостановлена. Если задание находится на карантине, состояние карантина будет очищено. Не создавайте скрипты для непрерывного вызова задания запуска во время его работы, так как это может привести к остановке работы службы. Используйте начните работу только в том случае, если задание приостановлено или находится на карантине. 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     |Directory.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |Не поддерживается. |
|Приложение                            |Application.ReadWrite.OwnedBy, Directory.ReadWrite.All | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a>Заголовки запроса

| Имя           | Тип    | Описание|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода. 

## <a name="response"></a>Отклик

В случае успешного ответа `204 No Content` возвращается ответ. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


