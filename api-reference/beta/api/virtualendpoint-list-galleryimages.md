---
title: Списки galleryImages
description: Список свойств и связей изображений галереи организации.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a0e932684c0f75112792a8082889c5dbe6a44dcc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126551"
---
# <a name="list-galleryimages"></a>Списки galleryImages

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список свойств и связей объектов [cloudPcGalleryImage.](../resources/cloudpcgalleryimage.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/galleryImages
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает `$select` параметры `$filter` запроса OData и помогает настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcgalleryimage"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/galleryImages
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcgalleryimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcgalleryimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcgalleryimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcgalleryimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-cloudpcgalleryimage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-cloudpcgalleryimage-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcGalleryImage",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cloudPcGalleryImage",
    "value": [
        {
            "id":"MicrosoftWindowsDesktop_windows-ent-cpc_19h2-ent-cpc-os",
            "displayName":"Windows 10 Enterprise + OS Optimizations 1909",
            "offerDisplayName":"Windows 10 Enterprise + OS Optimizations",
            "skuDisplayName":"1909",
            "publisher":"MicrosoftWindowsDesktop",
            "offer":"windows-ent-cpc",
            "sku":"19h2-ent-cpc-os",
            "recommendedSku":"light",
            "status":"supported",
            "sizeInGB":64,
            "startDate":"2019-11-12",
            "endDate":"2022-05-10",
            "expiredDate":"2022-11-10"
        },
        {
            "id":"MicrosoftWindowsDesktop_windows-ent-cpc_20h1-ent-cpc-os",
            "displayName":"Windows 10 Enterprise + OS Optimizations 2004",
            "offerDisplayName":"Windows 10 Enterprise + OS Optimizations",
            "skuDisplayName":"2004",
            "publisher":"MicrosoftWindowsDesktop",
            "offer":"windows-ent-cpc",
            "sku":"20h1-ent-cpc-os",
            "recommendedSku":"light",
            "status":"supported",
            "sizeInGB":64,
            "startDate":"2020-05-27",
            "endDate":"2021-12-14",
            "expiredDate":"2022-06-14"
        }
   ]
}
```
