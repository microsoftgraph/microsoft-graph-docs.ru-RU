---
title: Получение printJob
description: Получение свойств и связей задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 64d8d76a6c701210ad4556b2862b630b3dafb78c
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849118"
---
# <a name="get-printjob"></a><span data-ttu-id="7320e-103">Получение printJob</span><span class="sxs-lookup"><span data-stu-id="7320e-103">Get printJob</span></span>

<span data-ttu-id="7320e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7320e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7320e-105">Получение свойств и связей задания печати.</span><span class="sxs-lookup"><span data-stu-id="7320e-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="7320e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7320e-106">Permissions</span></span>
<span data-ttu-id="7320e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7320e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7320e-109">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) или [Получение](printershare-get.md) доступа к принтершаре в зависимости от того, используется ли принтер или принтершаре.</span><span class="sxs-lookup"><span data-stu-id="7320e-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="7320e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7320e-110">Permission type</span></span> | <span data-ttu-id="7320e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7320e-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7320e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7320e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7320e-113">PrintJob. ReadBasic, PrintJob. Read, PrintJob. ReadBasic. ALL, PrintJob. Read. ALL, PrintJob. Реадвритебасик, PrintJob. ReadWrite, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7320e-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="7320e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7320e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7320e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7320e-115">Not Supported.</span></span>|
|<span data-ttu-id="7320e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7320e-116">Application</span></span>| <span data-ttu-id="7320e-117">PrintJob. ReadBasic. ALL, PrintJob. Read. ALL, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7320e-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7320e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7320e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7320e-119">Чтобы получить задание с принтера:</span><span class="sxs-lookup"><span data-stu-id="7320e-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="7320e-120">Чтобы получить задание из общей папки принтера, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7320e-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7320e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7320e-121">Optional query parameters</span></span>
<span data-ttu-id="7320e-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7320e-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7320e-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7320e-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7320e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7320e-124">Request headers</span></span>
| <span data-ttu-id="7320e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7320e-125">Name</span></span>      |<span data-ttu-id="7320e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7320e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7320e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7320e-127">Authorization</span></span> | <span data-ttu-id="7320e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7320e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7320e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7320e-130">Request body</span></span>
<span data-ttu-id="7320e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7320e-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7320e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7320e-132">Response</span></span>
<span data-ttu-id="7320e-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7320e-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7320e-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="7320e-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="7320e-135">Пример 1: получение задания печати</span><span class="sxs-lookup"><span data-stu-id="7320e-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="7320e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7320e-136">Request</span></span>
<span data-ttu-id="7320e-137">Ниже приведен пример запроса на получение метаданных для задания печати.</span><span class="sxs-lookup"><span data-stu-id="7320e-137">The following is an example of a request to get metadata for a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="7320e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7320e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[<span data-ttu-id="7320e-139">C#</span><span class="sxs-lookup"><span data-stu-id="7320e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7320e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7320e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7320e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7320e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7320e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7320e-142">Response</span></span>
<span data-ttu-id="7320e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7320e-143">The following is an example of the response.</span></span>
><span data-ttu-id="7320e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7320e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 408

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "processingState": "completed",
    "processingStateDescription": "The print job has completed successfully and no further processing will take place."
  }
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="7320e-146">Пример 2: получение задания печати со списком задач</span><span class="sxs-lookup"><span data-stu-id="7320e-146">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="7320e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7320e-147">Request</span></span>
<span data-ttu-id="7320e-148">Ниже приведен запрос на получение задания печати и всех выполняемых или выполненных [задач](../resources/printtask.md) .</span><span class="sxs-lookup"><span data-stu-id="7320e-148">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="7320e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="7320e-149">Response</span></span>
<span data-ttu-id="7320e-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7320e-150">The following is an example of the response.</span></span>
><span data-ttu-id="7320e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7320e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 774

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs(tasks())/$entity",
  "id": "5182",
  "createdDateTime": "2020-06-30T17:18:52.3930472Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "processingState": "pendingHeld",
    "processingStateDescription": "The job is not a candidate for processing yet."
  },
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="7320e-153">Пример 3: получение задания печати и связанных с ним данных документа</span><span class="sxs-lookup"><span data-stu-id="7320e-153">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="7320e-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="7320e-154">Request</span></span>
<span data-ttu-id="7320e-155">Ниже приведен пример запроса на получение задания печати и связанных с ним данных документа.</span><span class="sxs-lookup"><span data-stu-id="7320e-155">The following is an example of a request to get a print job and its associated document data.</span></span>
# <a name="http"></a>[<span data-ttu-id="7320e-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="7320e-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="7320e-157">C#</span><span class="sxs-lookup"><span data-stu-id="7320e-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7320e-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7320e-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7320e-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7320e-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="7320e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="7320e-160">Response</span></span>
<span data-ttu-id="7320e-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7320e-161">The following is an example of the response.</span></span>
><span data-ttu-id="7320e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7320e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1688

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs(documents())/$entity",
  "id": "31216",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "ipAddress": null,
    "userPrincipalName": "",
    "oDataType": null
  },
  "status": {
  "processingState": "aborted",
  "processingStateDescription": "The print job has been aborted by a user or the printer and no further processing will take place."
  },
  "documents@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs('31216')/documents",
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604,
      "configuration": {
        "quality": "medium",
        "dpi": 300,
        "feedDirection": null,
        "orientation": "landscape",
        "duplexMode": "oneSided",
        "copies": 2,
        "colorMode": "color",
        "inputBin": null,
        "outputBin": null,
        "mediaSize": null,
        "mediaType": null,
        "finishings": [],
        "pagesPerSheet": null,
        "multipageLayout": "clockwiseFromTopLeft",
        "collate": true,
        "scaling": null,
        "fitPdfToPage": null,
        "margin": null,
        "pageRanges": []
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


