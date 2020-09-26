---
title: Страница через коллекцию с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию запросов API Microsoft Graph с помощью пакетов SDK Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: ef48af29a4cc0388c405e2a42894d98ce6c98010
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289491"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>Страница через коллекцию с помощью пакетов SDK Microsoft Graph

В целях повышения производительности коллекции сущностей часто делятся на страницы, и каждая страница возвращается с URL-адресом на следующую страницу. Класс **пажеитератор** упрощает использование постраничных коллекций. **Пажеитератор** обрабатывает перечисление текущей страницы и автоматический запрос последующих страниц.

## <a name="iterate-over-all-the-messages"></a>Итерация по всем сообщениям

В приведенном ниже примере показано, как выполняется итерация по всем сообщениям в почтовом ящике пользователя.

> [!TIP]
> В этом примере задается небольшой размер страницы с помощью `top` параметра для демонстрационных целей. Вы можете задать размер страницы до 999, чтобы свести к минимуму необходимое количество запросов.

### <a name="c"></a>[C#](#tab/csharp)

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

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

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

### <a name="java"></a>[Java](#tab/java)

```java
IMessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest()
    .select("Sender,Subject")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.GetCurrentPage();
  final IMessageCollectionRequestBuilder nextPage = messagesPage.GetNextPage();
  if(nextPage == null) {
    break;
  } else {
    messagePage = nextPage.buildRequest().get();
  }
}
```

---

## <a name="stopping-and-resuming-the-iteration"></a>Остановка и возобновление итерации

В некоторых сценариях требуется остановить процесс итерации, чтобы выполнить другие действия. Можно приостановить итерацию, вернувшись `false` из обратного вызова итерации. Итерацию можно возобновить, вызвав `resume` метод в **пажеитератор**.

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

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

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

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

### <a name="java"></a>[Java](#tab/java)

```java
// not supported in java SDK
```

---
<!-- markdownlint-enable MD024 -->
