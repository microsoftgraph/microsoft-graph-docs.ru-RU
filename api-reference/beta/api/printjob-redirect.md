---
title: 'printJob: перенаправление'
description: Перенаправляйте задание печати на другой принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8e31cfdff953feb689e7799954dd5ae260e9943e
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766422"
---
# <a name="printjob-redirect"></a><span data-ttu-id="28293-103">printJob: перенаправление</span><span class="sxs-lookup"><span data-stu-id="28293-103">printJob: redirect</span></span>

<span data-ttu-id="28293-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28293-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28293-105">[Перенаправляйте задание печати](../resources/printjob.md) на другой [принтер.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="28293-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="28293-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="28293-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="28293-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28293-107">Permissions</span></span>
<span data-ttu-id="28293-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="28293-110">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="28293-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="28293-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28293-111">Permission type</span></span> | <span data-ttu-id="28293-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28293-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="28293-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28293-113">Delegated (work or school account)</span></span>| <span data-ttu-id="28293-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28293-114">Not supported.</span></span> |
|<span data-ttu-id="28293-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28293-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28293-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28293-116">Not Supported.</span></span>|
|<span data-ttu-id="28293-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28293-117">Application</span></span>| <span data-ttu-id="28293-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="28293-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28293-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28293-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="28293-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28293-120">Request headers</span></span>
| <span data-ttu-id="28293-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28293-121">Name</span></span>          | <span data-ttu-id="28293-122">Описание</span><span class="sxs-lookup"><span data-stu-id="28293-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="28293-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28293-123">Authorization</span></span> | <span data-ttu-id="28293-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28293-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28293-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28293-126">Request body</span></span>
<span data-ttu-id="28293-127">В теле запроса укажи ID принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="28293-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="28293-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="28293-128">Property</span></span>     | <span data-ttu-id="28293-129">Тип</span><span class="sxs-lookup"><span data-stu-id="28293-129">Type</span></span>        | <span data-ttu-id="28293-130">Описание</span><span class="sxs-lookup"><span data-stu-id="28293-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28293-131">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="28293-131">destinationPrinterId</span></span>|<span data-ttu-id="28293-132">String</span><span class="sxs-lookup"><span data-stu-id="28293-132">String</span></span>|<span data-ttu-id="28293-133">ID принтера, на который должно быть перенаправлено задание печати.</span><span class="sxs-lookup"><span data-stu-id="28293-133">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="28293-134">configuration</span><span class="sxs-lookup"><span data-stu-id="28293-134">configuration</span></span>|<span data-ttu-id="28293-135">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="28293-135">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="28293-136">Обновленная конфигурация задания печати.</span><span class="sxs-lookup"><span data-stu-id="28293-136">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="28293-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="28293-137">Response</span></span>
<span data-ttu-id="28293-138">В случае успешного использования этот метод возвращает код отклика и объект `200 OK` [printJob](../resources/printjob.md) в очереди для принтера назначения.</span><span class="sxs-lookup"><span data-stu-id="28293-138">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="28293-139">Пример</span><span class="sxs-lookup"><span data-stu-id="28293-139">Example</span></span>
<span data-ttu-id="28293-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="28293-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="28293-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="28293-141">Request</span></span>
<span data-ttu-id="28293-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28293-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="28293-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="28293-143">HTTP</span></span>](#tab/http)
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

---


### <a name="response"></a><span data-ttu-id="28293-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="28293-144">Response</span></span>
<span data-ttu-id="28293-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28293-145">The following is an example of the response.</span></span> 
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


