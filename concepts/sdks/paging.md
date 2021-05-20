---
title: Страница через коллекцию с помощью SDKs Graph Microsoft
description: Содержит инструкции по созданию запросов Graph API Майкрософт с помощью SDKs Graph Microsoft.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 467a1114781105a0799724c8a072f19324948552
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546926"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a><span data-ttu-id="2c8b1-103">Страница через коллекцию с помощью SDKs Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="2c8b1-103">Page through a collection using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="2c8b1-104">По причинам производительности коллекции сущностями часто разбивают на страницы, и каждая страница возвращается с URL-адресом на следующую страницу.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-104">For performance reasons, collections of entities are often split into pages and each page is returned with a URL to the next page.</span></span> <span data-ttu-id="2c8b1-105">Класс **PageIterator** упрощает потребление страницных коллекций.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-105">The **PageIterator** class simplifies consuming of paged collections.</span></span> <span data-ttu-id="2c8b1-106">**PageIterator** обрабатывает переописание текущей страницы и автоматически запрашивает последующие страницы.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-106">**PageIterator** handles enumerating the current page and requesting subsequent pages automatically.</span></span>

## <a name="iterate-over-all-the-messages"></a><span data-ttu-id="2c8b1-107">Итерировать все сообщения</span><span class="sxs-lookup"><span data-stu-id="2c8b1-107">Iterate over all the messages</span></span>

<span data-ttu-id="2c8b1-108">В следующем примере показано итерирование всех сообщений в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-108">The following example shows iterating over all the messages in a user's mailbox.</span></span>

> [!TIP]
> <span data-ttu-id="2c8b1-109">В этом примере устанавливается небольшой размер страницы с `top` использованием параметра для демонстрационных целей.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-109">This example sets a small page size using the `top` parameter for demonstration purposes.</span></span> <span data-ttu-id="2c8b1-110">Можно установить размер страницы до 999, чтобы свести к минимуму количество необходимых запросов.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-110">You can set the page size up to 999 to minimize the number of requests that are necessary.</span></span>

### <a name="c"></a>[<span data-ttu-id="2c8b1-111">C#</span><span class="sxs-lookup"><span data-stu-id="2c8b1-111">C#</span></span>](#tab/csharp)

```csharp
var messages = await graphClient.Me.Messages
    .Request()
    .Select(e => new {
        e.Sender,
        e.Subject
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(graphClient, messages, (m) => {
        Console.WriteLine(m.Subject);
        return true;
    });

await pageIterator.IterateAsync();
```

### <a name="typescript"></a>[<span data-ttu-id="2c8b1-112">TypeScript</span><span class="sxs-lookup"><span data-stu-id="2c8b1-112">TypeScript</span></span>](#tab/typeScript)

```typescript
// Makes request to fetch mails list.
let response: PageCollection = await client
  .api("/me/messages?$top=10&$select=sender,subject")
  .get();

// A callback function to be called for every item in the collection.
// This call back should return boolean indicating whether not to
// continue the iteration process.
let callback: PageIteratorCallback = (data) => {
  console.log(data.subject);
  return true;
};

// Creating a new page iterator instance with client a graph client
// instance, page collection response from request and callback
let pageIterator = new PageIterator(client, response, callback);

// This iterates the collection until the nextLink is drained out.
await pageIterator.iterate();
```

### <a name="java"></a>[<span data-ttu-id="2c8b1-113">Java</span><span class="sxs-lookup"><span data-stu-id="2c8b1-113">Java</span></span>](#tab/java)

```java
final MessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest()
    .select("Sender,Subject")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.getCurrentPage();
  final MessageCollectionRequestBuilder nextPage = messagesPage.getNextPage();
  if(nextPage == null) {
    break;
  } else {
    messagePage = nextPage.buildRequest().get();
  }
}
```

---

## <a name="stopping-and-resuming-the-iteration"></a><span data-ttu-id="2c8b1-114">Остановка и повторное итерация</span><span class="sxs-lookup"><span data-stu-id="2c8b1-114">Stopping and resuming the iteration</span></span>

<span data-ttu-id="2c8b1-115">Некоторые сценарии требуют остановки процесса итерации для выполнения других действий.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-115">Some scenarios require stopping the iteration process in order to perform other actions.</span></span> <span data-ttu-id="2c8b1-116">Можно приостановить итерацию, возвращаясь из обратного `false` вызова итерации.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-116">It is possible to pause the iteration by returning `false` from the iteration callback.</span></span> <span data-ttu-id="2c8b1-117">Итерация может быть возобновлена путем вызова `resume` метода на **PageIterator**.</span><span class="sxs-lookup"><span data-stu-id="2c8b1-117">Iteration can be resumed by calling the `resume` method on the **PageIterator**.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="2c8b1-118">C#</span><span class="sxs-lookup"><span data-stu-id="2c8b1-118">C#</span></span>](#tab/csharp)

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
    .CreatePageIterator(graphClient, messages, (m) => {
        Console.WriteLine(m.Subject);
        count++;
        // If we've iterated over the limit,
        // stop the iteration by returning false
        return count < pauseAfter;
    });

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

### <a name="typescript"></a>[<span data-ttu-id="2c8b1-119">TypeScript</span><span class="sxs-lookup"><span data-stu-id="2c8b1-119">TypeScript</span></span>](#tab/typeScript)

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

### <a name="java"></a>[<span data-ttu-id="2c8b1-120">Java</span><span class="sxs-lookup"><span data-stu-id="2c8b1-120">Java</span></span>](#tab/java)

```java
// not supported in java SDK
```

---
<!-- markdownlint-enable MD024 -->
