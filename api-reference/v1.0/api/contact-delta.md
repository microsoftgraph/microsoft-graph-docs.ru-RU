---
title: 'contact: delta'
description: Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 08430a2ac67c793f924e0d0d396be2611b3428a7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316341"
---
# <a name="contact-delta"></a><span data-ttu-id="309ad-103">contact: delta</span><span class="sxs-lookup"><span data-stu-id="309ad-103">contact: delta</span></span>

<span data-ttu-id="309ad-104">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="309ad-104">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="309ad-p101">Вызов функции **delta** для контактов в папке похож на запрос GET. С тем исключением, что можно запрашивать добавочные изменения контактов в папке, правильно применяя [маркеры состояния](/graph/delta-query-overview) при этих вызовах. Это позволяет обслуживать и синхронизировать локальное хранилище контактов пользователя, не загружая каждый раз весь набор контактов с сервера.</span><span class="sxs-lookup"><span data-stu-id="309ad-p101">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="309ad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="309ad-107">Permissions</span></span>
<span data-ttu-id="309ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="309ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="309ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="309ad-110">Permission type</span></span>      | <span data-ttu-id="309ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="309ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="309ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="309ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="309ad-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="309ad-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="309ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="309ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="309ad-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="309ad-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="309ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="309ad-116">Application</span></span> | <span data-ttu-id="309ad-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="309ad-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="309ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="309ad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/{id}/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="309ad-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="309ad-119">Query parameters</span></span>

<span data-ttu-id="309ad-p103">Отслеживание изменений в контактах представляет собой цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего отклика в последующих запросах, так как в нем уже содержатся необходимые закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="309ad-p103">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="309ad-125">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="309ad-125">Query parameter</span></span>      | <span data-ttu-id="309ad-126">Тип</span><span class="sxs-lookup"><span data-stu-id="309ad-126">Type</span></span>   |<span data-ttu-id="309ad-127">Описание</span><span class="sxs-lookup"><span data-stu-id="309ad-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="309ad-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="309ad-128">$deltatoken</span></span> | <span data-ttu-id="309ad-129">string</span><span class="sxs-lookup"><span data-stu-id="309ad-129">string</span></span> | <span data-ttu-id="309ad-p104">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` при предыдущем вызове функции **delta** для той же коллекции контактов и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="309ad-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="309ad-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="309ad-132">$skiptoken</span></span> | <span data-ttu-id="309ad-133">string</span><span class="sxs-lookup"><span data-stu-id="309ad-133">string</span></span> | <span data-ttu-id="309ad-134">Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` при предыдущем вызове функции **delta** и указывает, что в коллекции контактов остаются не отслеженные изменения.</span><span class="sxs-lookup"><span data-stu-id="309ad-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="309ad-135">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="309ad-135">OData query parameters</span></span>

- <span data-ttu-id="309ad-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="309ad-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="309ad-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="309ad-138">Request headers</span></span>
| <span data-ttu-id="309ad-139">Имя</span><span class="sxs-lookup"><span data-stu-id="309ad-139">Name</span></span>       | <span data-ttu-id="309ad-140">Тип</span><span class="sxs-lookup"><span data-stu-id="309ad-140">Type</span></span> | <span data-ttu-id="309ad-141">Описание</span><span class="sxs-lookup"><span data-stu-id="309ad-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="309ad-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="309ad-142">Authorization</span></span>  | <span data-ttu-id="309ad-143">string</span><span class="sxs-lookup"><span data-stu-id="309ad-143">string</span></span>  | <span data-ttu-id="309ad-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="309ad-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="309ad-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="309ad-146">Content-Type</span></span>  | <span data-ttu-id="309ad-147">строка</span><span class="sxs-lookup"><span data-stu-id="309ad-147">string</span></span>  | <span data-ttu-id="309ad-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="309ad-p107">application/json. Required.</span></span> |
| <span data-ttu-id="309ad-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="309ad-150">Prefer</span></span> | <span data-ttu-id="309ad-151">string</span><span class="sxs-lookup"><span data-stu-id="309ad-151">string</span></span>  | <span data-ttu-id="309ad-p108">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="309ad-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="309ad-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="309ad-154">Response</span></span>

<span data-ttu-id="309ad-155">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="309ad-155">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="309ad-156">Пример</span><span class="sxs-lookup"><span data-stu-id="309ad-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="309ad-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="309ad-157">Request</span></span>
<span data-ttu-id="309ad-158">В следующем примере показано, как выполнить один вызов функции **delta**, использовать параметр `$select` для получения только свойства **displayName** каждого контакта и ограничить максимальное количество контактов в теле отклика двумя.</span><span class="sxs-lookup"><span data-stu-id="309ad-158">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="309ad-159">Чтобы отследить изменения контактов в папке, выполните один или несколько вызовов функции **delta** с правильными маркерами состояния, чтобы получить набор добавочных изменений с момента последнего разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="309ad-159">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="309ad-p109">Пример, в котором показано, как использовать маркеры состояния для отслеживания изменений сообщений в почтовой папке: [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages). Отслеживания контактов и отслеживания сообщений в папках отличаются, прежде всего, URL-адресами разностных запросов и возвращаемыми в откликах коллекциями (**contact** и **message** соответственно).</span><span class="sxs-lookup"><span data-stu-id="309ad-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 

# <a name="httptabhttp"></a>[<span data-ttu-id="309ad-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="309ad-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts/delta?$select=displayName
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="309ad-163">C#</span><span class="sxs-lookup"><span data-stu-id="309ad-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="309ad-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="309ad-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="309ad-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="309ad-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="309ad-166">Java</span><span class="sxs-lookup"><span data-stu-id="309ad-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="309ad-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="309ad-167">Response</span></span>
<span data-ttu-id="309ad-168">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="309ad-168">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="309ad-p110">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="309ad-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="309ad-171">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="309ad-171">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="309ad-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="309ad-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="309ad-174">См. также</span><span class="sxs-lookup"><span data-stu-id="309ad-174">See also</span></span>

- [<span data-ttu-id="309ad-175">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="309ad-175">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="309ad-176">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="309ad-176">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
