---
title: Объединение нескольких запросов в один вызов HTTP с помощью пакетной обработки JSON
description: 'Пакетная обработка JSON позволяет оптимизировать приложение, объединив несколько запросов в один объект JSON. Например, клиент может создать представление из таких несвязанных данных:'
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 4e1ad5734d0fefe2cdb7634e461ee9f297aae93e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721574"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a><span data-ttu-id="bbc35-104">Объединение нескольких запросов в один вызов HTTP с помощью пакетной обработки JSON</span><span class="sxs-lookup"><span data-stu-id="bbc35-104">Combine multiple requests in one HTTP call using JSON batching</span></span>

<span data-ttu-id="bbc35-p102">Пакетная обработка JSON позволяет оптимизировать приложение, объединив несколько запросов в один объект JSON. Например, клиент может создать представление из таких несвязанных данных:</span><span class="sxs-lookup"><span data-stu-id="bbc35-p102">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="bbc35-107">Изображение, хранящееся в OneDrive</span><span class="sxs-lookup"><span data-stu-id="bbc35-107">An image stored in OneDrive</span></span>
2. <span data-ttu-id="bbc35-108">Список задач Планировщика</span><span class="sxs-lookup"><span data-stu-id="bbc35-108">A list of Planner tasks</span></span>
3. <span data-ttu-id="bbc35-109">Календарь группы</span><span class="sxs-lookup"><span data-stu-id="bbc35-109">The calendar for a group</span></span>

<span data-ttu-id="bbc35-110">Объединение трех этих запросов в один может значительно снизить задержку в сети, ускорив работу приложения.</span><span class="sxs-lookup"><span data-stu-id="bbc35-110">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a><span data-ttu-id="bbc35-111">Первый пакетный запрос JSON</span><span class="sxs-lookup"><span data-stu-id="bbc35-111">First JSON batch request</span></span>

<span data-ttu-id="bbc35-p103">Сначала нужно создать пакетный запрос JSON для предыдущего примера. В этом сценарии отдельные запросы никак не зависят друг от друга, поэтому их можно поместить в пакетный запрос в любом порядке.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p103">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/v1.0/$batch
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
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

<span data-ttu-id="bbc35-p104">Ответы на пакетные запросы могут отображаться в другом порядке. Для сопоставления отдельных запросов и ответов можно использовать свойство `id`.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p104">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

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
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="bbc35-116">Формат запроса</span><span class="sxs-lookup"><span data-stu-id="bbc35-116">Request format</span></span>

<span data-ttu-id="bbc35-117">Пакетные запросы всегда отправляются с помощью метода `POST` в конечную точку `/$batch`.</span><span class="sxs-lookup"><span data-stu-id="bbc35-117">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="bbc35-p105">Текст пакетного запроса JSON состоит из одного объекта JSON с один обязательным свойством: `requests`. Свойство `requests` является массивом отдельных запросов. Для каждого отдельного запроса требуются свойства `id`, `method` и `url`.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p105">A JSON batch request body consists of a single JSON object with one required property: `requests`. The `requests` property is an array of individual requests. For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="bbc35-p106">Основная функция свойства `id` — сопоставление отдельных запросов и ответов. Это позволяет серверу обрабатывать запросы пакета в наиболее эффективном порядке.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p106">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="bbc35-p107">Свойства `method` и `url` отображаются в начале любого HTTP-запроса. method — это метод HTTP, а URL — это URL-адрес ресурса, на который обычно отправляется отдельный запрос.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p107">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="bbc35-125">Отдельные запросы также могут содержать свойства `headers` и `body`.</span><span class="sxs-lookup"><span data-stu-id="bbc35-125">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="bbc35-126">Обычно это объекты JSON, как показано в предыдущем примере.</span><span class="sxs-lookup"><span data-stu-id="bbc35-126">Both of these properties are typically JSON objects, as shown in the previous example.</span></span> <span data-ttu-id="bbc35-127">В некоторых случаях `body` может быть значением в кодировке URL Base64, а не объектом JSON (например, если body представляет собой изображение).</span><span class="sxs-lookup"><span data-stu-id="bbc35-127">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="bbc35-128">Когда в запрос включено свойство `body`, объект `headers` должен содержать значение для свойства `Content-Type`.</span><span class="sxs-lookup"><span data-stu-id="bbc35-128">When a `body` is included with the request, the `headers` object must contain a value for `Content-Type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="bbc35-129">Формат ответа</span><span class="sxs-lookup"><span data-stu-id="bbc35-129">Response format</span></span>

<span data-ttu-id="bbc35-p109">Формат ответа для пакетных запросов JSON почти такой же, как формат запроса. Ниже приведены основные различия.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p109">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="bbc35-132">Свойство в основном объекте JSON называется `responses`, а не `requests`.</span><span class="sxs-lookup"><span data-stu-id="bbc35-132">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="bbc35-133">Порядок отображения ответов и запросов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="bbc35-133">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="bbc35-p110">Вместо свойств `method` и `url` отдельные ответы содержат свойство `status`. Значение `status` — это код состояния HTTP.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p110">Rather than `method` and `url`, individual responses have a `status` property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="bbc35-p111">Пакетный ответ обычно содержит код состояния `200` или `400`. Если пакетный запрос имеет неправильный формат, код состояния — `400`. Если пакетный запрос пригоден для анализа, код состояния — `200`. Код состояния `200` пакетного ответа не указывает на успешное выполнение отдельных запросов в пакете. Именно поэтому у каждого отдельного ответа в свойстве `responses` есть код состояния.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p111">The status code on a batch response is typically `200` or `400`. If the batch request itself is malformed, the status code is `400`. If the batch request is parseable, the status code is `200`. A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded. This is why each individual response in the `responses` property has a status code.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="bbc35-141">Выстраивание последовательности запросов с помощью свойства dependsOn</span><span class="sxs-lookup"><span data-stu-id="bbc35-141">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="bbc35-p112">С помощью свойства `dependsOn` можно задать порядок выполнения запросов. Это свойство представляет собой массив строк, которые ссылаются на значения `id` различных отдельных запросов. Поэтому значения `id` должны быть уникальными. Например, в следующем запросе клиент указывает, что в первую очередь нужно выполнить запросы 1 и 3, затем запросы 2 и 4.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p112">Individual requests can be executed in a specified order by using the `dependsOn` property. This property is an array of strings that reference the `id` of a different individual request. For this reason, the values for `id` must be unique. For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

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

<span data-ttu-id="bbc35-146">Если отдельный запрос не будет выполнен, то любой зависящий от него запрос также не будет выполнен с кодом состояния `424` (ошибка зависимости).</span><span class="sxs-lookup"><span data-stu-id="bbc35-146">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="bbc35-147">Обход ограничения на длину URL-адреса с помощью пакетной обработки</span><span class="sxs-lookup"><span data-stu-id="bbc35-147">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="bbc35-p113">Еще один вариант использования пакетной обработки JSON — обход ограничения на длину URL-адреса. Если предложение фильтра сложное, длина URL-адреса может превышать ограничения, встроенные в браузеры или другие HTTP-клиенты. Для выполнения таких запросов можно использовать пакетную обработку JSON, так как длинные URL-адреса просто станут частью полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="bbc35-p113">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="bbc35-151">Известные проблемы</span><span class="sxs-lookup"><span data-stu-id="bbc35-151">Known issues</span></span>

<span data-ttu-id="bbc35-152">Список текущих ограничений, связанных с пакетной обработкой, см. в разделе [Известные проблемы][batching-known-issues].</span><span class="sxs-lookup"><span data-stu-id="bbc35-152">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="bbc35-153">См. также</span><span class="sxs-lookup"><span data-stu-id="bbc35-153">See also</span></span>

<span data-ttu-id="bbc35-154">Дополнительные сведения о формате пакетных запросов и ответов JSON см. в [спецификации формата JSON OData версии 4.01](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), раздел _Пакетные запросы и ответы_.</span><span class="sxs-lookup"><span data-stu-id="bbc35-154">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), section _Batch Requests and Responses_.</span></span>
