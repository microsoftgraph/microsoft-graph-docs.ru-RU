---
title: Get serviceHealthIssue
description: Извлечение свойств и связей объекта serviceHealthIssue.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 07a5d9e2952245b92592fe67c5f98c3664a96d5f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209008"
---
# <a name="get-servicehealthissue"></a>Get serviceHealthIssue
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение свойств и связей объекта [serviceHealthIssue.](../resources/servicehealthissue.md)

Эта операция извлекает указанную проблему со здоровьем службы для клиента. Операция возвращает ошибку, если проблема не существует для клиента.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ServiceHealth.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|ServiceHealth.Read.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [serviceHealthIssue](../resources/servicehealthissue.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO226784"],
  "name": "get_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO226784
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-servicehealthissue-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-servicehealthissue-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-servicehealthissue-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-servicehealthissue-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues/$entity",
  "startDateTime": "2020-11-14T08:15:00Z",
  "endDateTime": "2020-11-14T09:45:00Z",
  "lastModifiedDateTime": "2020-11-14T11:06:53.353Z",
  "title": "Intermittently unable to access some Microsoft 365 services",
  "id": "MO226784",
  "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
  "classification": "Advisory",
  "origin": "Microsoft",
  "status": "ServiceRestored",
  "service": "Microsoft 365 suite",
  "feature": "Access",
  "featureGroup": "Portal",
  "isResolved": true,
  "details": [],
  "posts": [
    {
      "createdDateTime": "2020-11-12T07:07:38.97Z",
      "postType": "Regular",
      "description": {
        "contentType": "Text",
        "content": "Title: Intermittently unable to invite partners to meetings using some Microsoft 365 services\n\nUser Impact: Users may have been intermittently unable to invite partners to meetings using some Microsoft 365 services."
      }
    }
  ]
}
```

