---
title: Get cloudPcGalleryImage
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcGalleryImage.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c1aafdfca8ecfbc9b067a63c16324f6eb791b708
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805584"
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
|Application|CloudPC.Read.All, CloudPC.ReadWrite.All|

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

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_cloudpcgalleryimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/galleryImages/{id}
```

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
