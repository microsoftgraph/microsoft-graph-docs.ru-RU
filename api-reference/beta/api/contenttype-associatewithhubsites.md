---
author: swapnil1993
title: 'contentType: associateWithHubSites'
description: Связать тип контента со списком узлов.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4248640f76252fbc9a7c8b446ff58c972fa4288f
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729425"
---
# <a name="contenttype-associatewithhubsites"></a>contentType: associateWithHubSites

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Связывать [тип контента][contentType] со списком сайтов-концентраторов.

>**Примечание:** Эта функция ограничена для клиентов, у SharePoint Syntex лицензии.
  

## <a name="permissions"></a>Разрешения  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------
|Делегированные (рабочая или учебная учетная запись) | Sites.Manage.All, Sites.FullControl.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|-|-|-|
|hubSiteUrls| Коллекция (строка) |Список пушечных URL-адресов для узлов, на которых необходимо применять тип контента. Обязательно.|
|propagateToExistingLists| Boolean |Если типы контента будут применяться в существующих списках на сайтах концентратора; в противном случае он будет применяться только к вновь `true` созданным спискам. 

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites
Content-Type: application/json

{
   "hubSiteUrls":[
      "https://graph.microsoft.com/beta/sites/id"
   ],
   "propagateToExistingLists":false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-associatewithhubsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-associatewithhubsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-associatewithhubsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-associatewithhubsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Отклик


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
