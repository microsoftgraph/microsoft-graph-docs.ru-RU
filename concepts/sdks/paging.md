---
title: Страница через коллекцию с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию запросов API Microsoft Graph с помощью пакетов SDK Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: e3cd656c5210739436ff9df68cfb700f264204de
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2020
ms.locfileid: "44052547"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a><span data-ttu-id="150a4-103">Страница через коллекцию с помощью пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="150a4-103">Page through a collection using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="150a4-104">В целях повышения производительности коллекции сущностей часто делятся на страницы, и каждая страница возвращается с URL-адресом на следующую страницу.</span><span class="sxs-lookup"><span data-stu-id="150a4-104">For performance reasons, collections of entities are often split into pages and each page is returned with a URL to the next page.</span></span> <span data-ttu-id="150a4-105">Класс **пажеитератор** упрощает использование постраничных коллекций.</span><span class="sxs-lookup"><span data-stu-id="150a4-105">The **PageIterator** class simplifies consuming of paged collections.</span></span> <span data-ttu-id="150a4-106">**Пажеитератор** обрабатывает перечисление текущей страницы и автоматический запрос последующих страниц.</span><span class="sxs-lookup"><span data-stu-id="150a4-106">**PageIterator** handles enumerating the current page and requesting subsequent pages automatically.</span></span>

## <a name="iterate-over-all-the-messages"></a><span data-ttu-id="150a4-107">Итерация по всем сообщениям</span><span class="sxs-lookup"><span data-stu-id="150a4-107">Iterate over all the messages</span></span>

<span data-ttu-id="150a4-108">В приведенном ниже примере показано, как выполняется итерация по всем сообщениям в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="150a4-108">The following example shows iterating over all the messages in a user's mailbox.</span></span>

> [!TIP]
> <span data-ttu-id="150a4-109">В этом примере задается небольшой размер страницы `top` с помощью параметра для демонстрационных целей.</span><span class="sxs-lookup"><span data-stu-id="150a4-109">This example sets a small page size using the `top` parameter for demonstration purposes.</span></span> <span data-ttu-id="150a4-110">Вы можете задать размер страницы до 999, чтобы свести к минимуму необходимое количество запросов.</span><span class="sxs-lookup"><span data-stu-id="150a4-110">You can set the page size up to 999 to minimize the number of requests that are necessary.</span></span>

### <a name="c"></a>[<span data-ttu-id="150a4-111">C#</span><span class="sxs-lookup"><span data-stu-id="150a4-111">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="150a4-112">TypeScript</span><span class="sxs-lookup"><span data-stu-id="150a4-112">TypeScript</span></span>](#tab/typeScript)

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

---

## <a name="stopping-and-resuming-the-iteration"></a><span data-ttu-id="150a4-113">Остановка и возобновление итерации</span><span class="sxs-lookup"><span data-stu-id="150a4-113">Stopping and resuming the iteration</span></span>

<span data-ttu-id="150a4-114">В некоторых сценариях требуется остановить процесс итерации, чтобы выполнить другие действия.</span><span class="sxs-lookup"><span data-stu-id="150a4-114">Some scenarios require stopping the iteration process in order to perform other actions.</span></span> <span data-ttu-id="150a4-115">Можно приостановить итерацию, вернувшись `false` из обратного вызова итерации.</span><span class="sxs-lookup"><span data-stu-id="150a4-115">It is possible to pause the iteration by returning `false` from the iteration callback.</span></span> <span data-ttu-id="150a4-116">Итерацию можно возобновить, вызвав `resume` метод в **пажеитератор**.</span><span class="sxs-lookup"><span data-stu-id="150a4-116">Iteration can be resumed by calling the `resume` method on the **PageIterator**.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="150a4-117">C#</span><span class="sxs-lookup"><span data-stu-id="150a4-117">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="150a4-118">TypeScript</span><span class="sxs-lookup"><span data-stu-id="150a4-118">TypeScript</span></span>](#tab/typeScript)

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

---
<!-- markdownlint-enable MD024 -->
