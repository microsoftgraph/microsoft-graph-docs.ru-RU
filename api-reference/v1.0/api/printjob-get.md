---
title: Получение printJob
description: Извлечение свойств и связей задания печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c97ffa869a14fbceedd0fc2e5b8f737792490d1c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518032"
---
# <a name="get-printjob"></a><span data-ttu-id="61e16-103">Получение printJob</span><span class="sxs-lookup"><span data-stu-id="61e16-103">Get printJob</span></span>
<span data-ttu-id="61e16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61e16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="61e16-105">Извлечение свойств и связей задания печати.</span><span class="sxs-lookup"><span data-stu-id="61e16-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="61e16-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61e16-106">Permissions</span></span>
<span data-ttu-id="61e16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="61e16-109">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет доступ [к принтеру Get](printer-get.md) или [Get printerShare](printershare-get.md) в зависимости от того, используется ли принтер или принтер.</span><span class="sxs-lookup"><span data-stu-id="61e16-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="61e16-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61e16-110">Permission type</span></span> | <span data-ttu-id="61e16-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61e16-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="61e16-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61e16-112">Delegated (work or school account)</span></span>| <span data-ttu-id="61e16-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e16-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="61e16-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61e16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61e16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61e16-115">Not Supported.</span></span>|
|<span data-ttu-id="61e16-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="61e16-116">Application</span></span>| <span data-ttu-id="61e16-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e16-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61e16-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61e16-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="61e16-119">Чтобы получить задание на принтере:</span><span class="sxs-lookup"><span data-stu-id="61e16-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="61e16-120">Чтобы получить задание из доли принтера:</span><span class="sxs-lookup"><span data-stu-id="61e16-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61e16-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61e16-121">Optional query parameters</span></span>
<span data-ttu-id="61e16-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="61e16-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="61e16-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="61e16-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="61e16-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61e16-124">Request headers</span></span>
|<span data-ttu-id="61e16-125">Имя</span><span class="sxs-lookup"><span data-stu-id="61e16-125">Name</span></span>|<span data-ttu-id="61e16-126">Описание</span><span class="sxs-lookup"><span data-stu-id="61e16-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61e16-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61e16-127">Authorization</span></span>|<span data-ttu-id="61e16-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61e16-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61e16-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61e16-130">Request body</span></span>
<span data-ttu-id="61e16-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61e16-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61e16-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e16-132">Response</span></span>

<span data-ttu-id="61e16-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект printJob](../resources/printjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="61e16-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61e16-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="61e16-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="61e16-135">Пример 1. Задание печати</span><span class="sxs-lookup"><span data-stu-id="61e16-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="61e16-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="61e16-136">Request</span></span>
<span data-ttu-id="61e16-137">Ниже приводится пример запроса на получения метаданных для задания печати.</span><span class="sxs-lookup"><span data-stu-id="61e16-137">The following is an example of a request to get metadata for a print job.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
```

#### <a name="response"></a><span data-ttu-id="61e16-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e16-138">Response</span></span>
<span data-ttu-id="61e16-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="61e16-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="61e16-140">Пример 2. Получить задание печати со списком задач</span><span class="sxs-lookup"><span data-stu-id="61e16-140">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="61e16-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="61e16-141">Request</span></span>
<span data-ttu-id="61e16-142">Ниже приводится запрос на выполнение задания [](../resources/printtask.md) печати и любые задачи, которые выполняются или выполняются.</span><span class="sxs-lookup"><span data-stu-id="61e16-142">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="61e16-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e16-143">Response</span></span>
<span data-ttu-id="61e16-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="61e16-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="61e16-145">Пример 3. Получить задание печати и связанные с ним данные документов</span><span class="sxs-lookup"><span data-stu-id="61e16-145">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="61e16-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="61e16-146">Request</span></span>
<span data-ttu-id="61e16-147">Ниже приводится пример запроса на задание печати и связанных с ним данных документов.</span><span class="sxs-lookup"><span data-stu-id="61e16-147">The following is an example of a request to get a print job and its associated document data.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=documents
```

#### <a name="response"></a><span data-ttu-id="61e16-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="61e16-148">Response</span></span>
<span data-ttu-id="61e16-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="61e16-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "documents@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs('5182')/documents",
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
