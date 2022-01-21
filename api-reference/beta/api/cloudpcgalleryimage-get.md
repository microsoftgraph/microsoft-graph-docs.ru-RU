---
title: Get cloudPcGalleryImage
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcGalleryImage.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 240289bcdfcb51ad1ec69e610e3a65c668324358
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131514"
---
# <a name="get-cloudpcgalleryimage"></a>Get cloudPcGalleryImage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями определенного [объекта cloudPcGalleryImage.](../resources/cloudpcgalleryimage.md)

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
GET /deviceManagement/virtualEndpoint/galleryImages/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает `$select` параметр запроса OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcgalleryimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/galleryImages/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcgalleryimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcgalleryimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcgalleryimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcgalleryimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-cloudpcgalleryimage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-cloudpcgalleryimage-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcGalleryImage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#cloudPcGalleryImage",
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
}

```
