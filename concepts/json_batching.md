# <a name="combine-multiple-requests-in-one-http-call-using-json-batching-preview"></a><span data-ttu-id="47859-101">Объединение нескольких запросов в один вызов HTTP с помощью пакетной обработки JSON (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="47859-101">Combine multiple requests in one HTTP call using JSON batching (preview)</span></span>

<span data-ttu-id="47859-p101">Пакетная обработка JSON позволяет оптимизировать приложение, объединив несколько запросов в один объект JSON. Например, клиент может создать представление из таких несвязанных данных:</span><span class="sxs-lookup"><span data-stu-id="47859-p101">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="47859-104">Изображение, хранящееся в OneDrive</span><span class="sxs-lookup"><span data-stu-id="47859-104">An image stored in OneDrive</span></span>
2. <span data-ttu-id="47859-105">Список задач Планировщика</span><span class="sxs-lookup"><span data-stu-id="47859-105">A list of Planner tasks</span></span>
3. <span data-ttu-id="47859-106">Календарь группы</span><span class="sxs-lookup"><span data-stu-id="47859-106">The calendar for a group</span></span>

<span data-ttu-id="47859-107">Объединение трех этих запросов в один может значительно снизить задержку в сети, ускорив работу приложения.</span><span class="sxs-lookup"><span data-stu-id="47859-107">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

## <a name="first-json-batch-request"></a><span data-ttu-id="47859-108">Первый пакетный запрос JSON</span><span class="sxs-lookup"><span data-stu-id="47859-108">First JSON batch request</span></span>

<span data-ttu-id="47859-p102">Сначала нужно создать пакетный запрос JSON для предыдущего примера. В этом сценарии отдельные запросы никак не зависят друг от друга, поэтому их можно поместить в пакетный запрос в любом порядке.</span><span class="sxs-lookup"><span data-stu-id="47859-p102">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/beta/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    }
  ]
}
```

<span data-ttu-id="47859-111">Ответы на пакетные запросы могут отображаться в другом порядке.</span><span class="sxs-lookup"><span data-stu-id="47859-111">Responses to the batched requests might appear in a different order. The  property can be used to correlate individual requests and responses.</span></span> <span data-ttu-id="47859-112">Для сопоставления отдельных запросов и ответов можно использовать свойство `id`.</span><span class="sxs-lookup"><span data-stu-id="47859-112">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="47859-113">Формат запроса</span><span class="sxs-lookup"><span data-stu-id="47859-113">Request format</span></span>

<span data-ttu-id="47859-114">Пакетные запросы всегда отправляются с помощью метода `POST` в конечную точку `/$batch`.</span><span class="sxs-lookup"><span data-stu-id="47859-114">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="47859-115">Текст пакетного запроса JSON состоит из одного объекта JSON с один обязательным свойством: `requests`.</span><span class="sxs-lookup"><span data-stu-id="47859-115">A JSON batch request body consists of a single JSON object with one required property: . The  property is an array of individual requests. For each individual request, the , , and  properties are required.</span></span> <span data-ttu-id="47859-116">Свойство `requests` является массивом отдельных запросов.</span><span class="sxs-lookup"><span data-stu-id="47859-116">The `requests` property is an array of individual requests.</span></span> <span data-ttu-id="47859-117">Для каждого отдельного запроса требуются свойства `id`, `method` и `url`.</span><span class="sxs-lookup"><span data-stu-id="47859-117">For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="47859-118">Основная функция свойства `id` — сопоставление отдельных запросов и ответов.</span><span class="sxs-lookup"><span data-stu-id="47859-118">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span> <span data-ttu-id="47859-119">Это позволяет серверу обрабатывать запросы пакета в наиболее эффективном порядке.</span><span class="sxs-lookup"><span data-stu-id="47859-119">The  property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="47859-120">Свойства `method` и `url` отображаются в начале любого HTTP-запроса.</span><span class="sxs-lookup"><span data-stu-id="47859-120">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span> <span data-ttu-id="47859-121">method — это метод HTTP, а URL — это URL-адрес ресурса, на который обычно отправляется отдельный запрос.</span><span class="sxs-lookup"><span data-stu-id="47859-121">The  and  properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="47859-122">Отдельные запросы также могут содержать свойства `headers` и `body`.</span><span class="sxs-lookup"><span data-stu-id="47859-122">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="47859-123">Обычно это объекты JSON.</span><span class="sxs-lookup"><span data-stu-id="47859-123">Both of these properties are typically JSON objects.</span></span> <span data-ttu-id="47859-124">В некоторых случаях `body` может быть значением в кодировке URL base64, а не объектом JSON — например, если body представляет собой изображение.</span><span class="sxs-lookup"><span data-stu-id="47859-124">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="47859-125">Когда в запрос включено свойство `body`, объект `headers` должен содержать значение для свойства `content-type`.</span><span class="sxs-lookup"><span data-stu-id="47859-125">When a `body` is included with the request, the `headers` object must contain a value for `content-type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="47859-126">Формат ответа</span><span class="sxs-lookup"><span data-stu-id="47859-126">Response format</span></span>

<span data-ttu-id="47859-p108">Формат ответа для пакетных запросов JSON почти такой же, как формат запроса. Ниже приведены основные различия.</span><span class="sxs-lookup"><span data-stu-id="47859-p108">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="47859-129">Свойство в основном объекте JSON называется `responses`, а не `requests`.</span><span class="sxs-lookup"><span data-stu-id="47859-129">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="47859-130">Порядок отображения ответов и запросов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="47859-130">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="47859-131">Вместо свойств `method` и `url` в отдельных ответах есть свойство `status`.</span><span class="sxs-lookup"><span data-stu-id="47859-131">Rather than `method` and `url`, individual responses have a `status` property.</span></span> <span data-ttu-id="47859-132">Значение `status` — это код состояния HTTP.</span><span class="sxs-lookup"><span data-stu-id="47859-132">Rather than  and , individual responses have a  property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="47859-133">Пакетный ответ обычно содержит код состояния `200` или `400`.</span><span class="sxs-lookup"><span data-stu-id="47859-133">The status code on a batch response is typically `200` or `400`.</span></span> <span data-ttu-id="47859-134">Если пакетный запрос имеет неправильный формат, код состояния — `400`.</span><span class="sxs-lookup"><span data-stu-id="47859-134">If the batch request itself is malformed, the status code is `400`.</span></span> <span data-ttu-id="47859-135">Если пакетный запрос пригоден для анализа, код состояния — `200`.</span><span class="sxs-lookup"><span data-stu-id="47859-135">If the batch request is parseable, the status code is `200`.</span></span> <span data-ttu-id="47859-136">Код состояния `200` пакетного ответа не указывает на успешное выполнение отдельных запросов в пакете.</span><span class="sxs-lookup"><span data-stu-id="47859-136">A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded.</span></span> <span data-ttu-id="47859-137">Именно поэтому у каждого отдельного ответа в свойстве `responses` есть код состояния.</span><span class="sxs-lookup"><span data-stu-id="47859-137">This is why each individual response in the `responses` property has a status code.</span></span>

<span data-ttu-id="47859-138">Кроме свойства `responses`, в пакетном ответе может быть свойство `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="47859-138">In addition to the `responses` property, there might be a `nextLink` property in the batch response.</span></span> <span data-ttu-id="47859-139">Это позволяет Microsoft Graph возвращать пакетный ответ сразу после выполнения каждого из отдельных запросов.</span><span class="sxs-lookup"><span data-stu-id="47859-139">This allows Microsoft Graph to return a batch response as soon as any of the individual requests has completed.</span></span> <span data-ttu-id="47859-140">Чтобы убедиться, что получены все отдельные ответы, продолжайте переходить по ссылке `nextLink`, пока она передается.</span><span class="sxs-lookup"><span data-stu-id="47859-140">To ensure that all individual responses have been received, continue to follow the `nextLink` as long as it exists.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="47859-141">Выстраивание последовательности запросов с помощью свойства dependsOn</span><span class="sxs-lookup"><span data-stu-id="47859-141">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="47859-142">С помощью свойства `dependsOn` можно задать порядок выполнения запросов.</span><span class="sxs-lookup"><span data-stu-id="47859-142">Individual requests can be executed in a specified order by using the `dependsOn` property.</span></span> <span data-ttu-id="47859-143">Это свойство представляет собой массив строк, которые ссылаются на значения `id` отдельных запросов.</span><span class="sxs-lookup"><span data-stu-id="47859-143">This property is an array of strings that reference the `id` of a different individual request.</span></span> <span data-ttu-id="47859-144">Поэтому значения `id` должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="47859-144">For this reason, the values for `id` must be unique.</span></span> <span data-ttu-id="47859-145">Например, в следующем запросе клиент указывает, что в первую очередь нужно выполнить запросы 1 и 3, затем запросы 2 и 4.</span><span class="sxs-lookup"><span data-stu-id="47859-145">For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

<span data-ttu-id="47859-146">Если отдельный запрос не будет выполнен, то любой зависящий от него запрос также не будет выполнен с кодом состояния `424` (ошибка зависимости).</span><span class="sxs-lookup"><span data-stu-id="47859-146">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="47859-147">Обход ограничения на длину URL-адреса с помощью пакетной обработки</span><span class="sxs-lookup"><span data-stu-id="47859-147">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="47859-p113">Еще один вариант использования пакетной обработки JSON — обход ограничения на длину URL-адреса. Если предложение фильтра сложное, длина URL-адреса может превышать ограничения, встроенные в браузеры или другие HTTP-клиенты. Для выполнения таких запросов можно использовать пакетную обработку JSON, так как длинные URL-адреса просто станут частью полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="47859-p113">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="47859-151">Известные проблемы</span><span class="sxs-lookup"><span data-stu-id="47859-151">Known issues</span></span>

<span data-ttu-id="47859-152">Список текущих ограничений, связанных с пакетной обработкой, см. в разделе [Известные проблемы][batching-known-issues].</span><span class="sxs-lookup"><span data-stu-id="47859-152">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: https://developer.microsoft.com/en-us/graph/docs/concepts/known_issues#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="47859-153">См. также</span><span class="sxs-lookup"><span data-stu-id="47859-153">See also</span></span>

<span data-ttu-id="47859-154">Дополнительные сведения о формате пакетных запросов и ответов JSON см. в [спецификации формата JSON OData версии 4.01][odata-4.01-json], раздел 18.</span><span class="sxs-lookup"><span data-stu-id="47859-154">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification][odata-4.01-json], section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span> <span data-ttu-id="47859-155">Обратите внимание, что это рабочая версия спецификации, но внесение изменений не планируется.</span><span class="sxs-lookup"><span data-stu-id="47859-155">For more information about the JSON batch request/response format, see the OData JSON Format Version 4.01 specification, section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span>

