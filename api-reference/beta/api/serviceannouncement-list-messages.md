---
title: Список сообщений
description: Извлекать ресурсы serviceUpdateMessage из свойства навигации сообщений.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 6cf564aa37fabe340283f144dcabf2004de85087
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396261"
---
# <a name="list-messages"></a>Список сообщений
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлекать [ресурсы serviceUpdateMessage](../resources/serviceupdatemessage.md) из свойства **навигации** сообщений.

Эта операция извлекает все сообщения обновления службы, которые существуют для клиента.

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
GET /admin/serviceAnnouncement/messages
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код отклика и коллекцию объектов [serviceUpdateMessage](../resources/serviceupdatemessage.md) в тексте отклика. Ответ paginated и каждая страница содержит 100 объектов.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceupdatemessage"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceupdatemessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceupdatemessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceupdatemessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceupdatemessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-serviceupdatemessage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-serviceupdatemessage-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages",
  "@odata.nextLink": "https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages?$skip=100",
  "value": [
    {
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
      "expiryDateTime": null,
      "details": [
        {
          "name": "ExternalLink",
          "value": "https://support.office.com/article/office-document-cache-settings-4b497318-ae4f-4a99-be42-b242b2e8b692"
        }
      ],
      "body": {
        "contentType": "Text",
        "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout......"
      },
      "viewPoint": null
    }
  ]
}
```

