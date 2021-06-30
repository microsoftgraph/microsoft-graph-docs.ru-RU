---
title: Get serviceUpdateMessage
description: Извлечение свойств и связей объекта serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 088985c53ec0887eb98e4619780143d8ac8805a8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208798"
---
# <a name="get-serviceupdatemessage"></a>Get serviceUpdateMessage
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение свойств и связей объекта [serviceUpdateMessage.](../resources/serviceupdatemessage.md)

Эта операция извлекает указанное сообщение обновления службы для клиента. Операция возвращает ошибку, если сообщение не существует для клиента.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ServiceMessage.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|ServiceMessage.Read.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}
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

В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [serviceUpdateMessage](../resources/serviceupdatemessage.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MC172851"],
  "name": "get_serviceupdatemessage"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC172851
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceupdatemessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceupdatemessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceupdatemessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceupdatemessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages/$entity",
    "startDateTime": "2019-02-01T18:51:00Z",
    "endDateTime": "2019-06-01T08:00:00Z",
    "lastModifiedDateTime": "2021-01-08T01:10:06.843Z",
    "title": "(Updated) New feature: Changes to PowerPoint and Word to open files faster",
    "id": "MC172851",
    "category": "StayInformed",
    "severity": "Normal",
    "tags": [
      "Updated message"
    ],
    "isMajorChange": true,
    "actionRequiredByDateTime": null,
    "services": [
      "SharePoint Online",
      "OneDrive for Business"
    ],
    "details": [
      {
        "name": "ExternalLink",
        "value": "https://support.office.com/article/office-document-cache-settings-4b497318-ae4f-4a99-be42-b242b2e8b692"
      }
    ],
    "body": {
      "contentType": "Text",
      "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout.  Thank you for your patience........"
    },
    "viewPoint": null
}
```
