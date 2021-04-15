---
title: Получение printJob
description: Извлечение свойств и связей задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c19306c2426603c39fb7892177be262feee03982
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766457"
---
# <a name="get-printjob"></a><span data-ttu-id="9ce91-103">Получение printJob</span><span class="sxs-lookup"><span data-stu-id="9ce91-103">Get printJob</span></span>

<span data-ttu-id="9ce91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ce91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ce91-105">Извлечение свойств и связей задания печати.</span><span class="sxs-lookup"><span data-stu-id="9ce91-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ce91-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce91-106">Permissions</span></span>
<span data-ttu-id="9ce91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9ce91-109">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет доступ [к принтеру Get](printer-get.md) или [Get printerShare](printershare-get.md) в зависимости от того, используется ли принтер или принтер.</span><span class="sxs-lookup"><span data-stu-id="9ce91-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="9ce91-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce91-110">Permission type</span></span> | <span data-ttu-id="9ce91-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ce91-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9ce91-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ce91-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9ce91-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce91-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="9ce91-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ce91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ce91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce91-115">Not Supported.</span></span>|
|<span data-ttu-id="9ce91-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ce91-116">Application</span></span>| <span data-ttu-id="9ce91-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce91-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ce91-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ce91-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="9ce91-119">Чтобы получить задание на принтере:</span><span class="sxs-lookup"><span data-stu-id="9ce91-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="9ce91-120">Чтобы получить задание из доли принтера:</span><span class="sxs-lookup"><span data-stu-id="9ce91-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ce91-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ce91-121">Optional query parameters</span></span>
<span data-ttu-id="9ce91-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce91-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ce91-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ce91-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ce91-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ce91-124">Request headers</span></span>
| <span data-ttu-id="9ce91-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9ce91-125">Name</span></span>      |<span data-ttu-id="9ce91-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce91-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ce91-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ce91-127">Authorization</span></span> | <span data-ttu-id="9ce91-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce91-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ce91-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ce91-130">Request body</span></span>
<span data-ttu-id="9ce91-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ce91-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9ce91-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce91-132">Response</span></span>
<span data-ttu-id="9ce91-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект printJob](../resources/printjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9ce91-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="9ce91-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ce91-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="9ce91-135">Пример 1. Задание печати</span><span class="sxs-lookup"><span data-stu-id="9ce91-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="9ce91-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce91-136">Request</span></span>
<span data-ttu-id="9ce91-137">Ниже приводится пример запроса на получения метаданных для задания печати.</span><span class="sxs-lookup"><span data-stu-id="9ce91-137">The following is an example of a request to get metadata for a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ce91-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce91-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[<span data-ttu-id="9ce91-139">C#</span><span class="sxs-lookup"><span data-stu-id="9ce91-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ce91-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ce91-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ce91-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ce91-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ce91-142">Java</span><span class="sxs-lookup"><span data-stu-id="9ce91-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9ce91-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce91-143">Response</span></span>
<span data-ttu-id="9ce91-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce91-144">The following is an example of the response.</span></span>
><span data-ttu-id="9ce91-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ce91-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ]
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="9ce91-147">Пример 2. Получить задание печати со списком задач</span><span class="sxs-lookup"><span data-stu-id="9ce91-147">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="9ce91-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce91-148">Request</span></span>
<span data-ttu-id="9ce91-149">Ниже приводится запрос на выполнение задания [](../resources/printtask.md) печати и любые задачи, которые выполняются или выполняются.</span><span class="sxs-lookup"><span data-stu-id="9ce91-149">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="9ce91-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce91-150">Response</span></span>
<span data-ttu-id="9ce91-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce91-151">The following is an example of the response.</span></span>
><span data-ttu-id="9ce91-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ce91-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ]
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "configuration": {    
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

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="9ce91-154">Пример 3. Получить задание печати и связанные с ним данные документов</span><span class="sxs-lookup"><span data-stu-id="9ce91-154">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="9ce91-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce91-155">Request</span></span>
<span data-ttu-id="9ce91-156">Ниже приводится пример запроса на задание печати и связанных с ним данных документов.</span><span class="sxs-lookup"><span data-stu-id="9ce91-156">The following is an example of a request to get a print job and its associated document data.</span></span>
# <a name="http"></a>[<span data-ttu-id="9ce91-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce91-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="9ce91-158">C#</span><span class="sxs-lookup"><span data-stu-id="9ce91-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ce91-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ce91-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ce91-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ce91-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ce91-161">Java</span><span class="sxs-lookup"><span data-stu-id="9ce91-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withdocumentdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="9ce91-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce91-162">Response</span></span>
<span data-ttu-id="9ce91-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce91-163">The following is an example of the response.</span></span>
><span data-ttu-id="9ce91-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ce91-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ]
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "configuration": {    
  },
  "documents@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs('31216')/documents",
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604
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


