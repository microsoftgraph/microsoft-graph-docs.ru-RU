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
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>Страница через коллекцию с использованием Microsoft Graph SDKs

По причинам производительности коллекции сущностей часто делятся на страницы, и каждая страница возвращается с URL на следующую страницу. Класс **PageIterator** упрощает потребление сборов страниц. **PageIterator** обрабатывает перечисление текущей страницы и автоматическое запрос последующих страниц.

## <a name="request-headers"></a>Заголовки запросов

Если вы отправляете какие-либо дополнительные заготовки запросов в ваш первоначальный запрос, эти заготовки не включены по умолчанию в последующие запросы страницы. Если эти загоны должны быть отправлены по последующим запросам, вы должны установить их явно.

## <a name="iterate-over-all-the-messages"></a>Итерировать все сообщения

В следующем примере показано итерирование всех сообщений в почтовом ящике пользователя.

> [!TIP]
> Этот пример устанавливает небольшой размер страницы, `top` используя параметр для демонстрационных целей. Вы можете установить размер страницы до 999, чтобы свести к минимуму количество запросов, которые необходимы.

### <a name="c"></a>[C#](#tab/csharp)

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

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

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

### <a name="java"></a>[Java](#tab/java)

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

## <a name="stopping-and-resuming-the-iteration"></a>Остановка и возобновление итерации

Некоторые сценарии требуют остановки процесса итерации для выполнения других действий. Можно приостановить итерацию, вернувшись `false` из итерации обратного вызова. Итерация может быть возобновлена, позвонив `resume` методу на **PageIterator**.

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
