---
title: 'printJob: перенаправление'
description: Перенаправляйте задание печати на другой принтер.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2f1415e4fc91fead1ed25f66867a3bd08f0dceb8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775978"
---
# <a name="printjob-redirect"></a><span data-ttu-id="6d0c1-103">printJob: перенаправление</span><span class="sxs-lookup"><span data-stu-id="6d0c1-103">printJob: redirect</span></span>
<span data-ttu-id="6d0c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d0c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6d0c1-105">[Перенаправляйте задание печати](../resources/printjob.md) на другой [принтер.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="6d0c1-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="6d0c1-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="6d0c1-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d0c1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d0c1-107">Permissions</span></span>
<span data-ttu-id="6d0c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d0c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6d0c1-110">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="6d0c1-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="6d0c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d0c1-111">Permission type</span></span> | <span data-ttu-id="6d0c1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d0c1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6d0c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d0c1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6d0c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-114">Not supported.</span></span> |
|<span data-ttu-id="6d0c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d0c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d0c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-116">Not Supported.</span></span>|
|<span data-ttu-id="6d0c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d0c1-117">Application</span></span>| <span data-ttu-id="6d0c1-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6d0c1-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d0c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d0c1-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="6d0c1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d0c1-120">Request headers</span></span>
|<span data-ttu-id="6d0c1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6d0c1-121">Name</span></span>|<span data-ttu-id="6d0c1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6d0c1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6d0c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d0c1-123">Authorization</span></span>|<span data-ttu-id="6d0c1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6d0c1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d0c1-126">Content-Type</span></span>|<span data-ttu-id="6d0c1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d0c1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d0c1-129">Request body</span></span>
<span data-ttu-id="6d0c1-130">В теле запроса укажи ID принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-130">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="6d0c1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d0c1-131">Property</span></span>     | <span data-ttu-id="6d0c1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6d0c1-132">Type</span></span>        | <span data-ttu-id="6d0c1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6d0c1-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d0c1-134">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="6d0c1-134">destinationPrinterId</span></span>|<span data-ttu-id="6d0c1-135">String</span><span class="sxs-lookup"><span data-stu-id="6d0c1-135">String</span></span>|<span data-ttu-id="6d0c1-136">ID принтера, на который должно быть перенаправлено задание печати.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-136">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="6d0c1-137">configuration</span><span class="sxs-lookup"><span data-stu-id="6d0c1-137">configuration</span></span>|<span data-ttu-id="6d0c1-138">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d0c1-138">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="6d0c1-139">Обновленная конфигурация задания печати.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-139">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="6d0c1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d0c1-140">Response</span></span>
<span data-ttu-id="6d0c1-141">В случае успешного использования этот метод возвращает код отклика и объект `200 OK` [printJob](../resources/printjob.md) в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-141">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="examples"></a><span data-ttu-id="6d0c1-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d0c1-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d0c1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d0c1-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6d0c1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d0c1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_redirect"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/redirect
Content-Type: application/json
Content-length: 128

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea",
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6d0c1-145">C#</span><span class="sxs-lookup"><span data-stu-id="6d0c1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d0c1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d0c1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d0c1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d0c1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d0c1-148">Java</span><span class="sxs-lookup"><span data-stu-id="6d0c1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d0c1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d0c1-149">Response</span></span>
<span data-ttu-id="6d0c1-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6d0c1-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea')/jobs/$entity",
  "id": "24123",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "processing",
    "description": "The print job is currently being processed by the printer.",
    "details": ["interpreting"]
  },
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

