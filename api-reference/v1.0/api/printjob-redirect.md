---
title: 'printJob: перенаправление'
description: Перенаправляйте задание печати на другой принтер.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 23e330a23c50e01f1d0e4ff5b05cadc3ae9b7cdc
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080073"
---
# <a name="printjob-redirect"></a><span data-ttu-id="a90bc-103">printJob: перенаправление</span><span class="sxs-lookup"><span data-stu-id="a90bc-103">printJob: redirect</span></span>
<span data-ttu-id="a90bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a90bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a90bc-105">[Перенаправляйте задание печати](../resources/printjob.md) на другой [принтер.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="a90bc-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="a90bc-106">Перенаправление задания печати будет успешным только в том случае, если в связанной работе печати имеется [printTask,](../resources/printTask.md) запущенный с триггера, созданного приложением-запросом. `processing`</span><span class="sxs-lookup"><span data-stu-id="a90bc-106">Redirecting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> 

<span data-ttu-id="a90bc-107">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="a90bc-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="a90bc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a90bc-108">Permissions</span></span>
<span data-ttu-id="a90bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a90bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a90bc-111">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="a90bc-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="a90bc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a90bc-112">Permission type</span></span> | <span data-ttu-id="a90bc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a90bc-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a90bc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a90bc-114">Delegated (work or school account)</span></span>| <span data-ttu-id="a90bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90bc-115">Not supported.</span></span> |
|<span data-ttu-id="a90bc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a90bc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a90bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90bc-117">Not Supported.</span></span>|
|<span data-ttu-id="a90bc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a90bc-118">Application</span></span>| <span data-ttu-id="a90bc-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a90bc-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a90bc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a90bc-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="a90bc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a90bc-121">Request headers</span></span>
|<span data-ttu-id="a90bc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a90bc-122">Name</span></span>|<span data-ttu-id="a90bc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a90bc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a90bc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a90bc-124">Authorization</span></span>|<span data-ttu-id="a90bc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a90bc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a90bc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a90bc-127">Content-Type</span></span>|<span data-ttu-id="a90bc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a90bc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a90bc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a90bc-130">Request body</span></span>
<span data-ttu-id="a90bc-131">В теле запроса укажи ID принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="a90bc-131">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="a90bc-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a90bc-132">Property</span></span>     | <span data-ttu-id="a90bc-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a90bc-133">Type</span></span>        | <span data-ttu-id="a90bc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a90bc-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a90bc-135">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="a90bc-135">destinationPrinterId</span></span>|<span data-ttu-id="a90bc-136">String</span><span class="sxs-lookup"><span data-stu-id="a90bc-136">String</span></span>|<span data-ttu-id="a90bc-137">ID принтера, на который должно быть перенаправлено задание печати.</span><span class="sxs-lookup"><span data-stu-id="a90bc-137">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="a90bc-138">configuration</span><span class="sxs-lookup"><span data-stu-id="a90bc-138">configuration</span></span>|<span data-ttu-id="a90bc-139">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="a90bc-139">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="a90bc-140">Обновленная конфигурация задания печати.</span><span class="sxs-lookup"><span data-stu-id="a90bc-140">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="a90bc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a90bc-141">Response</span></span>
<span data-ttu-id="a90bc-142">В случае успешного использования этот метод возвращает код отклика и объект `200 OK` [printJob](../resources/printjob.md) в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="a90bc-142">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="examples"></a><span data-ttu-id="a90bc-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="a90bc-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a90bc-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a90bc-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a90bc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a90bc-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a90bc-146">C#</span><span class="sxs-lookup"><span data-stu-id="a90bc-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a90bc-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a90bc-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a90bc-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a90bc-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a90bc-149">Java</span><span class="sxs-lookup"><span data-stu-id="a90bc-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a90bc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a90bc-150">Response</span></span>
<span data-ttu-id="a90bc-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a90bc-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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

