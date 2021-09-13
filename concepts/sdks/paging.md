---
title: Страница через коллекцию с помощью SDKs Graph Microsoft
description: Содержит инструкции по созданию запросов Graph API Майкрософт с помощью SDKs Graph Microsoft.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: ab76add730b0465ff7ef186f929573f6a360a1ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113457"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>Страница через коллекцию с помощью SDKs Graph Microsoft

По причинам производительности коллекции сущностями часто разбивают на страницы, и каждая страница возвращается с URL-адресом на следующую страницу. Класс **PageIterator** упрощает потребление страницных коллекций. **PageIterator** обрабатывает переописание текущей страницы и автоматически запрашивает последующие страницы.

## <a name="request-headers"></a>Заголовки запросов

Если вы отправляете дополнительные заглавные главы запросов в первоначальном запросе, эти заглавные по умолчанию не включаются в последующие запросы страниц. Если эти заголовки требуется отправлять в последующие запросы, их необходимо явно настроить.

## <a name="iterate-over-all-the-messages"></a>Итерировать все сообщения

В следующем примере показано итерирование всех сообщений в почтовом ящике пользователя.

> [!TIP]
> В этом примере устанавливается небольшой размер страницы с `top` использованием параметра для демонстрационных целей. Можно установить размер страницы до 999, чтобы свести к минимуму количество необходимых запросов.

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

## <a name="stopping-and-resuming-the-iteration"></a>Остановка и повторное итерация

Некоторые сценарии требуют остановки процесса итерации для выполнения других действий. Можно приостановить итерацию, возвращаясь из обратного `false` вызова итерации. Итерация может быть возобновлена путем вызова `resume` метода на **PageIterator**.

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
