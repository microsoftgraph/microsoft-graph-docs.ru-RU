---
title: 'todoTaskList: delta'
description: Получите набор ресурсов todoTaskList, которые были добавлены, удалены или удалены в Microsoft To Do.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 28ec2a0acaba340d27a9a83a1ac9ecc5b215bfbd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038763"
---
# <a name="todotasklist-delta"></a><span data-ttu-id="cba84-103">todoTaskList: delta</span><span class="sxs-lookup"><span data-stu-id="cba84-103">todoTaskList: delta</span></span>

<span data-ttu-id="cba84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cba84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cba84-105">Получите набор ресурсов [todoTaskList,](../resources/todotasklist.md) которые были добавлены, удалены или удалены в Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="cba84-105">Get a set of [todoTaskList](../resources/todotasklist.md) resources that have been added, deleted, or removed in Microsoft To Do.</span></span>

<span data-ttu-id="cba84-106">Вызов  функции дельты **для todoTaskList** похож на запрос GET, [](/graph/delta-query-overview) за исключением того, что при надлежащем применении маркеров состояния в одном или более из этих вызовов можно запрашивать дополнительные изменения в **todoTaskList**.</span><span class="sxs-lookup"><span data-stu-id="cba84-106">A **delta** function call for **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTaskList**.</span></span> <span data-ttu-id="cba84-107">Это позволяет поддерживать и синхронизировать локальный магазин **todoTaskList** пользователя без необходимости получать все **todoTaskList** с сервера каждый раз.</span><span class="sxs-lookup"><span data-stu-id="cba84-107">This allows you to maintain and synchronize a local store of a user's **todoTaskList** without having to fetch all the **todoTaskList** from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="cba84-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cba84-108">Permissions</span></span>
<span data-ttu-id="cba84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cba84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cba84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cba84-111">Permission type</span></span>      | <span data-ttu-id="cba84-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cba84-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cba84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cba84-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cba84-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba84-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cba84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cba84-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba84-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba84-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cba84-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cba84-117">Application</span></span> | <span data-ttu-id="cba84-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cba84-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="cba84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cba84-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a><span data-ttu-id="cba84-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="cba84-120">Query parameters</span></span>

<span data-ttu-id="cba84-121">Отслеживание изменений **в ресурсах todoTaskList** вызывает один или несколько вызовов функций **дельты.**</span><span class="sxs-lookup"><span data-stu-id="cba84-121">Tracking changes in **todoTaskList** resources incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="cba84-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="cba84-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="cba84-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="cba84-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="cba84-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="cba84-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="cba84-125">В последующих запросах просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные `nextLink` `deltaLink` и нужные параметры.</span><span class="sxs-lookup"><span data-stu-id="cba84-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="cba84-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="cba84-126">Query parameter</span></span>      | <span data-ttu-id="cba84-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cba84-127">Type</span></span>   |<span data-ttu-id="cba84-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cba84-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cba84-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="cba84-129">$deltatoken</span></span> | <span data-ttu-id="cba84-130">string</span><span class="sxs-lookup"><span data-stu-id="cba84-130">string</span></span> | <span data-ttu-id="cba84-131">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, должен вызывать ту же коллекцию `deltaLink` **todoTaskList,** что указывает на завершение этого раунда отслеживания изменений. </span><span class="sxs-lookup"><span data-stu-id="cba84-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same **todoTaskList** collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="cba84-132">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="cba84-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="cba84-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="cba84-133">$skiptoken</span></span> | <span data-ttu-id="cba84-134">string</span><span class="sxs-lookup"><span data-stu-id="cba84-134">string</span></span> | <span data-ttu-id="cba84-135">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же `nextLink` **собрании todoTaskList** необходимо отслеживать дальнейшие изменения. </span><span class="sxs-lookup"><span data-stu-id="cba84-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same **todoTaskList** collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="cba84-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="cba84-136">OData query parameters</span></span>

<span data-ttu-id="cba84-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="cba84-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="cba84-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cba84-139">Request headers</span></span>
| <span data-ttu-id="cba84-140">Имя</span><span class="sxs-lookup"><span data-stu-id="cba84-140">Name</span></span>       | <span data-ttu-id="cba84-141">Тип</span><span class="sxs-lookup"><span data-stu-id="cba84-141">Type</span></span> | <span data-ttu-id="cba84-142">Описание</span><span class="sxs-lookup"><span data-stu-id="cba84-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="cba84-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba84-143">Authorization</span></span>  | <span data-ttu-id="cba84-144">string</span><span class="sxs-lookup"><span data-stu-id="cba84-144">string</span></span>  | <span data-ttu-id="cba84-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cba84-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cba84-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cba84-147">Content-Type</span></span>  | <span data-ttu-id="cba84-148">string</span><span class="sxs-lookup"><span data-stu-id="cba84-148">string</span></span>  | <span data-ttu-id="cba84-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cba84-p107">application/json. Required.</span></span> |
| <span data-ttu-id="cba84-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="cba84-151">Prefer</span></span> | <span data-ttu-id="cba84-152">string</span><span class="sxs-lookup"><span data-stu-id="cba84-152">string</span></span>  | <span data-ttu-id="cba84-p108">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cba84-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cba84-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba84-155">Response</span></span>

<span data-ttu-id="cba84-156">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [коллекции todoTaskList](../resources/todotasklist.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cba84-156">If successful, this method returns a `200 OK` response code and [todoTaskList](../resources/todotasklist.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba84-157">Пример</span><span class="sxs-lookup"><span data-stu-id="cba84-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="cba84-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="cba84-158">Request</span></span>
<span data-ttu-id="cba84-159">В следующем примере показано, как сделать начальный вызов функции дельты и ограничить максимальное число **todoTaskList** в теле ответа 2. </span><span class="sxs-lookup"><span data-stu-id="cba84-159">The following example shows how to make an initial **delta** function call, and limit the maximum number of **todoTaskList** in the response body to 2.</span></span>

<span data-ttu-id="cba84-160">Чтобы отслеживать изменения **в todoTaskList,** необходимо  сделать один или несколько вызовов функции дельты с соответствующими маркерами состояния, чтобы получить набор дополнительных изменений после последнего запроса дельты.</span><span class="sxs-lookup"><span data-stu-id="cba84-160">To track changes in the **todoTaskList**, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="cba84-161">Основные различия между отслеживанием **todoTaskList** и отслеживанием ресурсов **todoTask** в списке находятся в URL-адресах запроса запроса дельты и ответов на запросы, возвращающие **коллекции todoTaskList,** а не **todoTask.**</span><span class="sxs-lookup"><span data-stu-id="cba84-161">The main differences between tracking **todoTaskList** and tracking **todoTask** resources in a list are in the delta query request URLs, and the query responses returning **todoTaskList** rather than **todoTask** collections.</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a><span data-ttu-id="cba84-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba84-162">Response</span></span>

<span data-ttu-id="cba84-163">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="cba84-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="cba84-p109">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="cba84-p109">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="cba84-166">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="cba84-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="cba84-167">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cba84-167">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="cba84-168">См. также</span><span class="sxs-lookup"><span data-stu-id="cba84-168">See also</span></span>

- [<span data-ttu-id="cba84-169">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cba84-169">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)

