---
title: 'printJob: перенаправление'
description: Перенаправляйте задание печати на другой принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 916725283b86c59907ddd89e5441902fa0f8c756
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080178"
---
# <a name="printjob-redirect"></a><span data-ttu-id="0f2c9-103">printJob: перенаправление</span><span class="sxs-lookup"><span data-stu-id="0f2c9-103">printJob: redirect</span></span>

<span data-ttu-id="0f2c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f2c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f2c9-105">[Перенаправляйте задание печати](../resources/printjob.md) на другой [принтер.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="0f2c9-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="0f2c9-106">Перенаправление задания печати будет успешным только в том случае, если в связанной работе печати имеется [printTask,](../resources/printTask.md) запущенный с триггера, созданного приложением-запросом. `processing`</span><span class="sxs-lookup"><span data-stu-id="0f2c9-106">Redirecting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> 

<span data-ttu-id="0f2c9-107">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="0f2c9-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f2c9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f2c9-108">Permissions</span></span>
<span data-ttu-id="0f2c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f2c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0f2c9-111">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="0f2c9-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="0f2c9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f2c9-112">Permission type</span></span> | <span data-ttu-id="0f2c9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f2c9-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0f2c9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f2c9-114">Delegated (work or school account)</span></span>| <span data-ttu-id="0f2c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-115">Not supported.</span></span> |
|<span data-ttu-id="0f2c9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f2c9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f2c9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-117">Not Supported.</span></span>|
|<span data-ttu-id="0f2c9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f2c9-118">Application</span></span>| <span data-ttu-id="0f2c9-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0f2c9-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f2c9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f2c9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="0f2c9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f2c9-121">Request headers</span></span>
| <span data-ttu-id="0f2c9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0f2c9-122">Name</span></span>          | <span data-ttu-id="0f2c9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0f2c9-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f2c9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f2c9-124">Authorization</span></span> | <span data-ttu-id="0f2c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f2c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f2c9-127">Request body</span></span>
<span data-ttu-id="0f2c9-128">В теле запроса укажи ID принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-128">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="0f2c9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f2c9-129">Property</span></span>     | <span data-ttu-id="0f2c9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f2c9-130">Type</span></span>        | <span data-ttu-id="0f2c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f2c9-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f2c9-132">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="0f2c9-132">destinationPrinterId</span></span>|<span data-ttu-id="0f2c9-133">String</span><span class="sxs-lookup"><span data-stu-id="0f2c9-133">String</span></span>|<span data-ttu-id="0f2c9-134">ID принтера, на который должно быть перенаправлено задание печати.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-134">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="0f2c9-135">configuration</span><span class="sxs-lookup"><span data-stu-id="0f2c9-135">configuration</span></span>|<span data-ttu-id="0f2c9-136">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f2c9-136">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="0f2c9-137">Обновленная конфигурация задания печати.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-137">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="0f2c9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f2c9-138">Response</span></span>
<span data-ttu-id="0f2c9-139">В случае успешного использования этот метод возвращает код отклика и объект `200 OK` [printJob](../resources/printjob.md) в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-139">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="0f2c9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0f2c9-140">Example</span></span>
<span data-ttu-id="0f2c9-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-141">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="0f2c9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f2c9-142">Request</span></span>
<span data-ttu-id="0f2c9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0f2c9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f2c9-144">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="0f2c9-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f2c9-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

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
# <a name="c"></a>[<span data-ttu-id="0f2c9-146">C#</span><span class="sxs-lookup"><span data-stu-id="0f2c9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f2c9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f2c9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f2c9-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f2c9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f2c9-149">Java</span><span class="sxs-lookup"><span data-stu-id="0f2c9-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="0f2c9-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f2c9-150">Response</span></span>
<span data-ttu-id="0f2c9-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f2c9-151">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 437

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#printJob",
  "@odata.type": "#microsoft.graph.printJob",
  "id": "44354",
  "createdDateTime": "2020-06-30T17:19:09Z",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


