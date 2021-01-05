---
title: Лучшие методики для API Excel в Microsoft Graph
description: Список лучших методик и примеров для API Excel в Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c7e72c4c6480c75d3080d32c2984e6d0f594c409
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754070"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a><span data-ttu-id="a1d3b-103">Best practices for working with the Excel API in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a1d3b-103">Best practices for working with the Excel API in Microsoft Graph</span></span>

<span data-ttu-id="a1d3b-104">В этой статье данная статья содержит рекомендации по работе с API Excel в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-104">This article provides recommendations for working with the Excel APIs in Microsoft Graph.</span></span>

## <a name="manage-sessions-in-the-most-efficient-way"></a><span data-ttu-id="a1d3b-105">Управление сеансами наиболее эффективным способом</span><span class="sxs-lookup"><span data-stu-id="a1d3b-105">Manage sessions in the most efficient way</span></span>

<span data-ttu-id="a1d3b-106">Если в течение определенного периода времени необходимо сделать несколько вызовов, рекомендуется создать сеанс и передать его ИД с каждым запросом.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-106">If you have more than one call to make within a certain period of time, we recommend that you create a session and pass the session ID with each request.</span></span> <span data-ttu-id="a1d3b-107">Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-107">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> <span data-ttu-id="a1d3b-108">Таким образом, вы можете использовать API Excel наиболее эффективным способом.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-108">By doing so, you can use the Excel APIs in the most efficient way.</span></span>

<span data-ttu-id="a1d3b-109">В следующем примере показано, как добавить новый номер в таблицу и найти одну запись в книге с помощью этого подхода.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-109">The following example shows you how to add a new number to a table and then find one record in a workbook using this approach.</span></span>

### <a name="step-1-create-a-session"></a><span data-ttu-id="a1d3b-110">Шаг 1. Создание сеанса</span><span class="sxs-lookup"><span data-stu-id="a1d3b-110">Step 1: Create a session</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-111">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-111">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
#### <a name="response"></a><span data-ttu-id="a1d3b-112">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-112">Response</span></span>

<span data-ttu-id="a1d3b-113">Ниже приводится успешный ответ.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-113">The following is a successful response.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a><span data-ttu-id="a1d3b-114">Шаг 2. Добавление новой строки в таблицу</span><span class="sxs-lookup"><span data-stu-id="a1d3b-114">Step 2: Add a new row to the table</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-115">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/Table1/rows/add
Content-type: application/json
workbook-session-id: {session-id}

{
  "values": [[“east”, “pear”, 4]]
}
```

#### <a name="response"></a><span data-ttu-id="a1d3b-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-116">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 42

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a><span data-ttu-id="a1d3b-117">Шаг 3. Найди значение в обновленной таблице</span><span class="sxs-lookup"><span data-stu-id="a1d3b-117">Step 3: Look up a value in the updated table</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-118">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/functions/vlookup
Content-type: application/json
workbook-session-id: {session-id}

{
    "lookupValue":"pear",
    "tableArray":{"Address":"Sheet1!B2:C7"},
    "colIndexNum":2,
    "rangeLookup":false
}
```

#### <a name="response"></a><span data-ttu-id="a1d3b-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-119">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json

{
    "value": 5
}
```

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a><span data-ttu-id="a1d3b-120">Шаг 4. Закроем сеанс после завершения всех запросов</span><span class="sxs-lookup"><span data-stu-id="a1d3b-120">Step 4: Close the session after all the requests are completed</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-121">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{
}
```

#### <a name="response"></a><span data-ttu-id="a1d3b-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-122">Response</span></span>

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="a1d3b-123">Дополнительные сведения см. в [сведениях о создании сеанса](/graph/api/workbook-createsession?view=graph-rest-1.0) [и закрытии сеанса.](/graph/api/workbook-closesession?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="a1d3b-123">For more details, see [Create session](/graph/api/workbook-createsession?view=graph-rest-1.0) and [Close session](/graph/api/workbook-closesession?view=graph-rest-1.0).</span></span>

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a><span data-ttu-id="a1d3b-124">Работа с API, которые занять много времени</span><span class="sxs-lookup"><span data-stu-id="a1d3b-124">Working with APIs that take a long time to complete</span></span>

<span data-ttu-id="a1d3b-125">Вы можете заметить, что для выполнения некоторых операций необходимо определенное время; например, открытие большой книги.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-125">You might notice that some operations take an indeterminate amount time to complete; for example, opening a large workbook.</span></span> <span data-ttu-id="a1d3b-126">При ожидании ответа на эти запросы легко получить время ожидания.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-126">It is easy to hit timeout while waiting for the response to these requests.</span></span> <span data-ttu-id="a1d3b-127">Чтобы устранить эту проблему, мы предоставляем долгосрочный шаблон операций.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-127">To resolve this issue, we provide the long-running operation pattern.</span></span> <span data-ttu-id="a1d3b-128">При использовании этого шаблона вам не нужно беспокоиться о времени простоя запроса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-128">When you use this pattern, you don't need to worry about the timeout for the request.</span></span>

<span data-ttu-id="a1d3b-129">В настоящее время для API Создания сеанса Excel в Microsoft Graph включен долгосрочный шаблон операций.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-129">Currently, the session creation Excel API in Microsoft Graph has the long-running operation pattern enabled.</span></span> <span data-ttu-id="a1d3b-130">Этот шаблон состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="a1d3b-130">This pattern involves the following steps:</span></span>

1. <span data-ttu-id="a1d3b-131">Добавьте в запрос заголок, чтобы указать, что это долго работа при перенастройке `Prefer: respond-async` сеанса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-131">Add a `Prefer: respond-async` header to the request to indicate that it is a long-running operation when you crate a session.</span></span>
2. <span data-ttu-id="a1d3b-132">При длительной операции возвращается ответ вместе с заготовом расположением для `202 Accepted` получения состояния операции.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-132">A long-running operation will return a `202 Accepted` response along with a Location header to retrieve the operation status.</span></span> <span data-ttu-id="a1d3b-133">Если создание сеанса завершается через несколько секунд, он возвращает обычный ответ на создание сеанса вместо использования длительной операции.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-133">If the session creation completes in several seconds, it will return a regular create session response instead of using the long-running operation pattern.</span></span>
3. <span data-ttu-id="a1d3b-134">С помощью `202 Accepted` отклика можно получить состояние операции в указанном расположении.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-134">With the `202 Accepted` response, you can retrieve the operation status at the specified location.</span></span> <span data-ttu-id="a1d3b-135">Значения состояния операции: `notStarted` , , , и `running` `succeeded` `failed` .</span><span class="sxs-lookup"><span data-stu-id="a1d3b-135">Operation status values include `notStarted`, `running`, `succeeded`, and `failed`.</span></span>
4. <span data-ttu-id="a1d3b-136">После завершения операции можно получить результат создания сеанса по указанному URL-адресу в успешном ответе.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-136">After the operation completes, you can get the session creation result through the specified URL in the succeeded response.</span></span>

<span data-ttu-id="a1d3b-137">В следующем примере создается сеанс с использованием шаблона длительных операций.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-137">The following example creates a session using the long-running operation pattern.</span></span>

### <a name="initial-request-to-create-session"></a><span data-ttu-id="a1d3b-138">Начальный запрос на создание сеанса</span><span class="sxs-lookup"><span data-stu-id="a1d3b-138">Initial request to create session</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-139">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a><span data-ttu-id="a1d3b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-140">Response</span></span>
<span data-ttu-id="a1d3b-141">Шаблон длительных операций возвращает `202 Accepted` ответ, аналогичный следующему.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-141">The long-running operation pattern will return a `202 Accepted` response similar to the following.</span></span>

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

<span data-ttu-id="a1d3b-142">В некоторых случаях, если создание успешно в течение нескольких секунд, оно не будет вводить шаблон длительной операции; вместо этого он возвращается в качестве обычного сеанса создания, и успешный запрос возвращает `201 Created` ответ.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-142">In some cases, if the creation succeeds within seconds, it won't enter the long-running operation pattern; instead, it returns as a regular create session and the successful request will return a `201 Created` response.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

<span data-ttu-id="a1d3b-143">В следующем примере показан ответ при сбойе запроса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-143">The following example shows the response when the request fails.</span></span>

><span data-ttu-id="a1d3b-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-144">**Note:** The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json

{
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": "internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

### <a name="poll-status-of-the-long-running-create-session"></a><span data-ttu-id="a1d3b-145">Опрос состояния продолжительного сеанса создания</span><span class="sxs-lookup"><span data-stu-id="a1d3b-145">Poll status of the long-running create session</span></span>


<span data-ttu-id="a1d3b-146">С помощью шаблона длительной операции можно получить состояние создания в указанном расположении с помощью следующего запроса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-146">With the long-running operation pattern, you can get the creation status at specified location by using the following request.</span></span> <span data-ttu-id="a1d3b-147">Рекомендуемый интервал опроса составляет около 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-147">The suggested interval to poll status is around 30 seconds.</span></span> <span data-ttu-id="a1d3b-148">Максимальный интервал не должен быть больше 4 минут.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-148">The maximum interval should be no more than 4 minutes.</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-149">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a><span data-ttu-id="a1d3b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-150">Response</span></span>

<span data-ttu-id="a1d3b-151">Ниже приводится ответ, когда операция находится в состоянии `running` .</span><span class="sxs-lookup"><span data-stu-id="a1d3b-151">The following is the response when the operation has a status of `running`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

<span data-ttu-id="a1d3b-152">Ниже приводится ответ, когда операция находится в состоянии `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="a1d3b-152">The following is the response when the operation status is `succeeded`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

<span data-ttu-id="a1d3b-153">Ниже приводится ответ, когда операция находится в состоянии `failed` .</span><span class="sxs-lookup"><span data-stu-id="a1d3b-153">The following is the response when the operation status is `failed`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": {operation-id},
  "status": "failed",
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": ""internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

<span data-ttu-id="a1d3b-154">Дополнительные сведения об ошибках см. в [кодах ошибок.](workbook-error-codes.md#error-code)</span><span class="sxs-lookup"><span data-stu-id="a1d3b-154">For more details about errors, see [Error codes](workbook-error-codes.md#error-code).</span></span>

### <a name="acquire-session-information"></a><span data-ttu-id="a1d3b-155">Получение сведений о сеансе</span><span class="sxs-lookup"><span data-stu-id="a1d3b-155">Acquire session information</span></span>

#### <a name="request"></a><span data-ttu-id="a1d3b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d3b-156">Request</span></span>

<span data-ttu-id="a1d3b-157">С состоянием ,вы можете получить сведения о созданном сеансе с помощью следующего `succeeded` `resourceLocation` запроса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-157">With a status of `succeeded`, you can get the created session information through `resourceLocation` with a request similar to the following.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

#### <a name="response"></a><span data-ttu-id="a1d3b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d3b-158">Response</span></span>
<span data-ttu-id="a1d3b-159">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-159">The following is the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "id-value",
    "persistChanges": true
}
```

><span data-ttu-id="a1d3b-160">**Примечание.** Получение сведений о сеансе зависит от исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-160">**Note:** Acquire session information depends on the initial request.</span></span> <span data-ttu-id="a1d3b-161">Вам не нужно получать результат, если исходный запрос не возвращает тело ответа.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-161">You don't need to acquire the result if the initial request doesn't return a response body.</span></span>
