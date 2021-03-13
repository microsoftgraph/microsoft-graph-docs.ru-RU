---
title: Обновление printJob
description: Задание обновления печати
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 885190ea6a23ed6c5408f7476f5a4f10463ae012
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768779"
---
# <a name="update-printjob"></a><span data-ttu-id="188c0-103">Обновление printJob</span><span class="sxs-lookup"><span data-stu-id="188c0-103">Update printJob</span></span>
<span data-ttu-id="188c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="188c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="188c0-105">Обновление [задания печати](../resources/printjob.md).</span><span class="sxs-lookup"><span data-stu-id="188c0-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="188c0-106">Только свойство **конфигурации** может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="188c0-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="188c0-107">Обновление задания печати будет успешным только в том случае, если в связанной работе печати имеется [printTask,](../resources/printTask.md) запущенный с триггера, созданного `processing` приложением-запросом.</span><span class="sxs-lookup"><span data-stu-id="188c0-107">Updating a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="188c0-108">Подробные сведения о регистрации триггера задач см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="188c0-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="188c0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="188c0-109">Permissions</span></span>
<span data-ttu-id="188c0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="188c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="188c0-112">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку на универсальную печать, либо разрешение принтера.Read.All или Printer.ReadWrite.All, а также одно из разрешений, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="188c0-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="188c0-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="188c0-113">Permission type</span></span> | <span data-ttu-id="188c0-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="188c0-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="188c0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="188c0-115">Delegated (work or school account)</span></span>| <span data-ttu-id="188c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="188c0-116">Not supported.</span></span> |
|<span data-ttu-id="188c0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="188c0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="188c0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="188c0-118">Not Supported.</span></span>|
|<span data-ttu-id="188c0-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="188c0-119">Application</span></span>| <span data-ttu-id="188c0-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="188c0-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="188c0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="188c0-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}/jobs/{printJobId}
```

## <a name="request-headers"></a><span data-ttu-id="188c0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="188c0-122">Request headers</span></span>
|<span data-ttu-id="188c0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="188c0-123">Name</span></span>|<span data-ttu-id="188c0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="188c0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="188c0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="188c0-125">Authorization</span></span>|<span data-ttu-id="188c0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="188c0-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="188c0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="188c0-128">Content-Type</span></span>|<span data-ttu-id="188c0-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="188c0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="188c0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="188c0-131">Request body</span></span>
<span data-ttu-id="188c0-132">В теле запроса укажи значения соответствующих [полей printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="188c0-132">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="188c0-133">Существующие свойства, не включенные в тело запроса, будут поддерживать прежние значения.</span><span class="sxs-lookup"><span data-stu-id="188c0-133">Existing properties that are not included in the request body will maintain their previous values.</span></span> 

<span data-ttu-id="188c0-134">Только свойство **конфигурации** может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="188c0-134">Only the **configuration** property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="188c0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="188c0-135">Response</span></span>

<span data-ttu-id="188c0-136">В случае успешной работы этот метод возвращает код ответа с обновленным объектом `200 OK` [printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="188c0-136">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="188c0-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="188c0-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="188c0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="188c0-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="188c0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="188c0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printjob"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
Content-Type: application/json
Content-length: 376

{
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
# <a name="c"></a>[<span data-ttu-id="188c0-140">C#</span><span class="sxs-lookup"><span data-stu-id="188c0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="188c0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="188c0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="188c0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="188c0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="188c0-143">Java</span><span class="sxs-lookup"><span data-stu-id="188c0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="188c0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="188c0-144">Response</span></span>
<span data-ttu-id="188c0-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="188c0-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
  "id": "44353",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet."
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

