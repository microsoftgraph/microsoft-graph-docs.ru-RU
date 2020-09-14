---
title: Рекомендации по использованию API Excel в Microsoft Graph
description: Перечисление рекомендаций и примеров для API Excel в Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c113d162874c3121e97534b8d098d1c52a24fe77
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651297"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a><span data-ttu-id="8a9dd-103">Рекомендации по работе с API Excel в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a9dd-103">Best practices for working with the Excel API in Microsoft Graph</span></span>

<span data-ttu-id="8a9dd-104">В этой статье приводятся рекомендации по работе с API Excel в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-104">This article provides recommendations for working with the Excel APIs in Microsoft Graph.</span></span>

## <a name="manage-sessions-in-the-most-efficient-way"></a><span data-ttu-id="8a9dd-105">Наиболее эффективный способ управления сеансами</span><span class="sxs-lookup"><span data-stu-id="8a9dd-105">Manage sessions in the most efficient way</span></span>

<span data-ttu-id="8a9dd-106">При наличии нескольких вызовов, которые необходимо выполнить в течение определенного периода времени, рекомендуется создать сеанс и передать ему идентификатор сеанса с каждым запросом.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-106">If you have more than one call to make within a certain period of time, we recommend that you create a session and pass the session ID with each request.</span></span> <span data-ttu-id="8a9dd-107">Чтобы представить сеанс в API, используйте заголовок `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-107">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> <span data-ttu-id="8a9dd-108">Таким образом, вы можете использовать API Excel наиболее эффективным способом.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-108">By doing so, you can use the Excel APIs in the most efficient way.</span></span>

<span data-ttu-id="8a9dd-109">В приведенном ниже примере показано, как добавить в таблицу новый номер, а затем найти одну запись в книге, используя этот подход.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-109">The following example shows you how to add a new number to a table and then find one record in a workbook using this approach.</span></span>

### <a name="step-1-create-a-session"></a><span data-ttu-id="8a9dd-110">Шаг 1: Создание сеанса</span><span class="sxs-lookup"><span data-stu-id="8a9dd-110">Step 1: Create a session</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-111">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-111">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
#### <a name="response"></a><span data-ttu-id="8a9dd-112">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-112">Response</span></span>

<span data-ttu-id="8a9dd-113">Ниже приведен успешный ответ.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-113">The following is a successful response.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a><span data-ttu-id="8a9dd-114">Шаг 2: Добавление новой строки в таблицу</span><span class="sxs-lookup"><span data-stu-id="8a9dd-114">Step 2: Add a new row to the table</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-115">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/Table1/rows/add
Content-type: application/json
workbook-session-id: {session-id}

{
  "values": [[“east”, “pear”, 4]]
}
```

#### <a name="response"></a><span data-ttu-id="8a9dd-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-116">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 42

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a><span data-ttu-id="8a9dd-117">Шаг 3: поиск значения в обновленной таблице</span><span class="sxs-lookup"><span data-stu-id="8a9dd-117">Step 3: Look up a value in the updated table</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-118">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8a9dd-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-119">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json

{
    "value": 5
}
```

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a><span data-ttu-id="8a9dd-120">Шаг 4: закрытие сеанса после завершения всех запросов</span><span class="sxs-lookup"><span data-stu-id="8a9dd-120">Step 4: Close the session after all the requests are completed</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-121">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{
}
```

#### <a name="response"></a><span data-ttu-id="8a9dd-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-122">Response</span></span>

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="8a9dd-123">Более подробную информацию можно узнать в статье [Создание сеанса](/graph/api/workbook-createsession?view=graph-rest-1.0) и [закрытие сеанса](/graph/api/workbook-closesession?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="8a9dd-123">For more details, see [Create session](/graph/api/workbook-createsession?view=graph-rest-1.0) and [Close session](/graph/api/workbook-closesession?view=graph-rest-1.0).</span></span>

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a><span data-ttu-id="8a9dd-124">Работа с API, для выполнения которых требуется длительное время</span><span class="sxs-lookup"><span data-stu-id="8a9dd-124">Working with APIs that take a long time to complete</span></span>

<span data-ttu-id="8a9dd-125">Вы можете заметить, что для выполнения некоторых операций требуется неопределенное количество времени; Например, открытие большой книги.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-125">You might notice that some operations take an indeterminate amount time to complete; for example, opening a large workbook.</span></span> <span data-ttu-id="8a9dd-126">При ожидании ответа на эти запросы очень легко достичь времени ожидания ответа.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-126">It is easy to hit timeout while waiting for the response to these requests.</span></span> <span data-ttu-id="8a9dd-127">Чтобы устранить эту проблему, мы предоставим долгосрочный шаблон операции.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-127">To resolve this issue, we provide the long-running operation pattern.</span></span> <span data-ttu-id="8a9dd-128">При использовании этого шаблона не нужно беспокоиться об истечении времени ожидания запроса.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-128">When you use this pattern, you don't need to worry about the timeout for the request.</span></span>

<span data-ttu-id="8a9dd-129">В настоящее время в интерфейсе API для создания сеансов в Microsoft Graph включен шаблон длительного выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-129">Currently, the session creation Excel API in Microsoft Graph has the long-running operation pattern enabled.</span></span> <span data-ttu-id="8a9dd-130">Этот шаблон состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="8a9dd-130">This pattern involves the following steps:</span></span>

1. <span data-ttu-id="8a9dd-131">Добавьте `Prefer: respond-async` заголовок в запрос, чтобы указать, что это длительная операция, выполняемая при создании сеанса.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-131">Add a `Prefer: respond-async` header to the request to indicate that it is a long-running operation when you crate a session.</span></span>
2. <span data-ttu-id="8a9dd-132">При длительной операции возвращается `202 Accepted` ответ вместе с заголовком Location для получения состояния операции.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-132">A long-running operation will return a `202 Accepted` response along with a Location header to retrieve the operation status.</span></span> <span data-ttu-id="8a9dd-133">Если создание сеанса завершается через несколько секунд, возвращается обычный ответ на создание сеанса, а не использование долгосрочного шаблона операции.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-133">If the session creation completes in several seconds, it will return a regular create session response instead of using the long-running operation pattern.</span></span>
3. <span data-ttu-id="8a9dd-134">С `202 Accepted` ответом вы можете получить состояние операции в указанном расположении.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-134">With the `202 Accepted` response, you can retrieve the operation status at the specified location.</span></span> <span data-ttu-id="8a9dd-135">Значения состояния операции включают `notStarted` , `running` , `succeeded` и `failed` .</span><span class="sxs-lookup"><span data-stu-id="8a9dd-135">Operation status values include `notStarted`, `running`, `succeeded`, and `failed`.</span></span>
4. <span data-ttu-id="8a9dd-136">После завершения операции вы можете получить результат создания сеанса по указанному URL-адресу в ответе, успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-136">After the operation completes, you can get the session creation result through the specified URL in the succeeded response.</span></span>

<span data-ttu-id="8a9dd-137">В следующем примере создается сеанс с использованием долгосрочного шаблона операции.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-137">The following example creates a session using the long-running operation pattern.</span></span>

### <a name="initial-request-to-create-session"></a><span data-ttu-id="8a9dd-138">Первоначальный запрос на создание сеанса</span><span class="sxs-lookup"><span data-stu-id="8a9dd-138">Initial request to create session</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-139">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a><span data-ttu-id="8a9dd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-140">Response</span></span>
<span data-ttu-id="8a9dd-141">Шаблон длительной операции возвращает `202 Accepted` ответ, аналогичный приведенному ниже.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-141">The long-running operation pattern will return a `202 Accepted` response similar to the following.</span></span>

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

<span data-ttu-id="8a9dd-142">В некоторых случаях, если создание прошло успешно в течение нескольких секунд, оно не будет вводить шаблон длительной операции; Вместо этого он возвращает как обычный сеанс создания, а успешный запрос возвращает `201 Created` ответ.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-142">In some cases, if the creation succeeds within seconds, it won't enter the long-running operation pattern; instead, it returns as a regular create session and the successful request will return a `201 Created` response.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

<span data-ttu-id="8a9dd-143">В следующем примере показан ответ при сбое запроса.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-143">The following example shows the response when the request fails.</span></span>

><span data-ttu-id="8a9dd-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="poll-status-of-the-long-running-create-session"></a><span data-ttu-id="8a9dd-145">Состояние опроса длительно выполняемого сеанса создания</span><span class="sxs-lookup"><span data-stu-id="8a9dd-145">Poll status of the long-running create session</span></span>


<span data-ttu-id="8a9dd-146">С помощью шаблона длительной операции вы можете получить состояние создания в указанном расположении с помощью следующего запроса.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-146">With the long-running operation pattern, you can get the creation status at specified location by using the following request.</span></span> <span data-ttu-id="8a9dd-147">Рекомендуемый интервал для состояния опроса составляет около 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-147">The suggested interval to poll status is around 30 seconds.</span></span> <span data-ttu-id="8a9dd-148">Максимальный интервал не должен превышать 4 минуты.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-148">The maximum interval should be no more than 4 minutes.</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-149">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a><span data-ttu-id="8a9dd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-150">Response</span></span>

<span data-ttu-id="8a9dd-151">Ниже приведен ответ, в котором находится состояние операции `running` .</span><span class="sxs-lookup"><span data-stu-id="8a9dd-151">The following is the response when the operation has a status of `running`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

<span data-ttu-id="8a9dd-152">Ниже приведен ответ на состояние операции `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="8a9dd-152">The following is the response when the operation status is `succeeded`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

<span data-ttu-id="8a9dd-153">Ниже приведен ответ на состояние операции `failed` .</span><span class="sxs-lookup"><span data-stu-id="8a9dd-153">The following is the response when the operation status is `failed`.</span></span>

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

<span data-ttu-id="8a9dd-154">Более подробную информацию об ошибках можно узнать в статье [коды ошибок](/concepts/workbook-error-codes.md)</span><span class="sxs-lookup"><span data-stu-id="8a9dd-154">For more details about errors, see [Error codes](/concepts/workbook-error-codes.md)</span></span>

### <a name="acquire-session-information"></a><span data-ttu-id="8a9dd-155">Получение сведений о сеансе</span><span class="sxs-lookup"><span data-stu-id="8a9dd-155">Acquire session information</span></span>

#### <a name="request"></a><span data-ttu-id="8a9dd-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a9dd-156">Request</span></span>

<span data-ttu-id="8a9dd-157">С состоянием `succeeded` можно получить сведения о созданном сеансе с помощью `resourceLocation` запроса, аналогичного приведенному ниже.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-157">With a status of `succeeded`, you can get the created session information through `resourceLocation` with a request similar to the following.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

#### <a name="response"></a><span data-ttu-id="8a9dd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a9dd-158">Response</span></span>
<span data-ttu-id="8a9dd-159">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-159">The following is the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "id-value",
    "persistChanges": true
}
```

><span data-ttu-id="8a9dd-160">**Примечание:** Получение сведений о сеансе зависит от первоначального запроса.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-160">**Note:** Acquire session information depends on the initial request.</span></span> <span data-ttu-id="8a9dd-161">Нет необходимости приобретать результат, если исходный запрос не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="8a9dd-161">You don't need to acquire the result if the initial request doesn't return a response body.</span></span>
