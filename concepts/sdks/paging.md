---
title: Страница через коллекцию с использованием Microsoft Graph SDKs
description: Предоставляет инструкции по созданию Graph API с использованием microsoft Graph SDKs.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d06a23e5c1e53042192fe3fe8b4c8e3fe13c488d
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579664"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a><span data-ttu-id="fb8a3-103">Страница через коллекцию с использованием Microsoft Graph SDKs</span><span class="sxs-lookup"><span data-stu-id="fb8a3-103">Page through a collection using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="fb8a3-104">По причинам производительности коллекции сущностей часто делятся на страницы, и каждая страница возвращается с URL на следующую страницу.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-104">For performance reasons, collections of entities are often split into pages and each page is returned with a URL to the next page.</span></span> <span data-ttu-id="fb8a3-105">Класс **PageIterator** упрощает потребление сборов страниц.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-105">The **PageIterator** class simplifies consuming of paged collections.</span></span> <span data-ttu-id="fb8a3-106">**PageIterator** обрабатывает перечисление текущей страницы и автоматическое запрос последующих страниц.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-106">**PageIterator** handles enumerating the current page and requesting subsequent pages automatically.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb8a3-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb8a3-107">Request headers</span></span>

<span data-ttu-id="fb8a3-108">Если вы отправляете какие-либо дополнительные заготовки запросов в ваш первоначальный запрос, эти заготовки не включены по умолчанию в последующие запросы страницы.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-108">If you send any additional request headers in your initial request, those headers are not included by default in subsequent page requests.</span></span> <span data-ttu-id="fb8a3-109">Если эти загоны должны быть отправлены по последующим запросам, вы должны установить их явно.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-109">If those headers need to be sent on subsequent requests, you must set them explicitly.</span></span>

## <a name="iterate-over-all-the-messages"></a><span data-ttu-id="fb8a3-110">Итерировать все сообщения</span><span class="sxs-lookup"><span data-stu-id="fb8a3-110">Iterate over all the messages</span></span>

<span data-ttu-id="fb8a3-111">В следующем примере показано итерирование всех сообщений в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-111">The following example shows iterating over all the messages in a user's mailbox.</span></span>

> [!TIP]
> <span data-ttu-id="fb8a3-112">Этот пример устанавливает небольшой размер страницы, `top` используя параметр для демонстрационных целей.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-112">This example sets a small page size using the `top` parameter for demonstration purposes.</span></span> <span data-ttu-id="fb8a3-113">Вы можете установить размер страницы до 999, чтобы свести к минимуму количество запросов, которые необходимы.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-113">You can set the page size up to 999 to minimize the number of requests that are necessary.</span></span>

### <a name="c"></a>[<span data-ttu-id="fb8a3-114">C#</span><span class="sxs-lookup"><span data-stu-id="fb8a3-114">C#</span></span>](#tab/csharp)

```csharp
var messages = await graphClient.Me.Messages
    .Request()
    .Header("Prefer", "outlook.body-content-type=\"text\"")
    .Select(e => new {
        e.Sender,
        e.Subject,
        e.Body
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(
        graphClient,
        messages,
        // Callback executed for each item in
        // the collection
        (m) =>
        {
            Console.WriteLine(m.Subject);
            return true;
        },
        // Used to configure subsequent page
        // requests
        (req) =>
        {
            // Re-add the header to subsequent requests
            req.Header("Prefer", "outlook.body-content-type=\"text\"");
            return req;
        }
    );

await pageIterator.IterateAsync();
```

### <a name="typescript"></a>[<span data-ttu-id="fb8a3-115">TypeScript</span><span class="sxs-lookup"><span data-stu-id="fb8a3-115">TypeScript</span></span>](#tab/typeScript)

```typescript
// Makes request to fetch mails list.
let response: PageCollection = await client
  .api("/me/messages?$top=10&$select=sender,subject,body")
  .header('Prefer', 'outlook.body-content-type="text"')
  .get();

// A callback function to be called for every item in the collection.
// This call back should return boolean indicating whether not to
// continue the iteration process.
let callback: PageIteratorCallback = (data) => {
  console.log(data.subject);
  return true;
};

// A set of request options to be applied to
// all subsequent page requests
let requestOptions: GraphRequestOptions = {
  // Re-add the header to subsequent requests
  headers: {
    'Prefer': 'outlook.body-content-type="text"'
  }
};

// Creating a new page iterator instance with client a graph client
// instance, page collection response from request and callback
let pageIterator = new PageIterator(client, response, callback, requestOptions);

// This iterates the collection until the nextLink is drained out.
await pageIterator.iterate();
```

### <a name="java"></a>[<span data-ttu-id="fb8a3-116">Java</span><span class="sxs-lookup"><span data-stu-id="fb8a3-116">Java</span></span>](#tab/java)

```java
final MessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""))
    .select("Sender,Subject,Body")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.getCurrentPage();
  final MessageCollectionRequestBuilder nextPage = messagesPage.getNextPage();
  if(nextPage == null) {
    break;
  } else {
    messagePage = nextPage.buildRequest(
        // Re-add the header to subsequent requests
        new HeaderOption("Prefer", "outlook.body-content-type=\"text\"")
    ).get();
  }
}
```

---

## <a name="stopping-and-resuming-the-iteration"></a><span data-ttu-id="fb8a3-117">Остановка и возобновление итерации</span><span class="sxs-lookup"><span data-stu-id="fb8a3-117">Stopping and resuming the iteration</span></span>

<span data-ttu-id="fb8a3-118">Некоторые сценарии требуют остановки процесса итерации для выполнения других действий.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-118">Some scenarios require stopping the iteration process in order to perform other actions.</span></span> <span data-ttu-id="fb8a3-119">Можно приостановить итерацию, вернувшись `false` из итерации обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-119">It is possible to pause the iteration by returning `false` from the iteration callback.</span></span> <span data-ttu-id="fb8a3-120">Итерация может быть возобновлена, позвонив `resume` методу на **PageIterator**.</span><span class="sxs-lookup"><span data-stu-id="fb8a3-120">Iteration can be resumed by calling the `resume` method on the **PageIterator**.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="fb8a3-121">C#</span><span class="sxs-lookup"><span data-stu-id="fb8a3-121">C#</span></span>](#tab/csharp)

```csharp
int count = 0;
int pauseAfter = 25;

var messages = await graphClient.Me.Messages
    .Request()
    .Select(e => new {
        e.Sender,
        e.Subject
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(
        graphClient,
        messages,
        (m) =>
        {
            Console.WriteLine(m.Subject);
            count++;
            // If we've iterated over the limit,
            // stop the iteration by returning false
            return count < pauseAfter;
        }
    );

await pageIterator.IterateAsync();

while (pageIterator.State != PagingState.Complete)
{
    Console.WriteLine("Iteration paused for 5 seconds...");
    Thread.Sleep(5000);
    // Reset count
    count = 0;
    await pageIterator.ResumeAsync();
}
```

### <a name="typescript"></a>[<span data-ttu-id="fb8a3-122">TypeScript</span><span class="sxs-lookup"><span data-stu-id="fb8a3-122">TypeScript</span></span>](#tab/typeScript)

```typescript
let count: number = 0;
let pauseAfter: number = 25;

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();

let callback: PageIteratorCallback = (data) => {
  result = `${result}${data.subject}\n`;
  console.log(data.subject);
  count++;

  // If we've iterated over the limit,
  // stop the iteration by returning false
  return count < pauseAfter;
};

let pageIterator = new PageIterator(client, response, callback);
await pageIterator.iterate();

while (!pageIterator.isComplete()) {
  console.log('Iteration paused for 5 seconds...');
  await new Promise(resolve => setTimeout(resolve, 5000));

  // Reset count
  count = 0;
  await pageIterator.resume();
}
```

### <a name="java"></a>[<span data-ttu-id="fb8a3-123">Java</span><span class="sxs-lookup"><span data-stu-id="fb8a3-123">Java</span></span>](#tab/java)

```java
// not supported in java SDK
```

---
<!-- markdownlint-enable MD024 -->
