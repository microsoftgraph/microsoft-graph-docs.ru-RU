---
title: 'todoTask: delta'
description: Получение набора ресурсов todoTask, которые были добавлены в указанный объект todoTaskList, обновлены в указанном объекте todoTaskList, обновлены в нем или удалены из него.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 56f114cc8bb24b7cfb250839a3711459cafd6104
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850070"
---
# <a name="todotask-delta"></a><span data-ttu-id="f4766-103">todoTask: delta</span><span class="sxs-lookup"><span data-stu-id="f4766-103">todoTask: delta</span></span>

<span data-ttu-id="f4766-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4766-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4766-105">Получение набора ресурсов [todoTask,](../resources/todotask.md) которые были добавлены в указанный объект todoTaskList, обновлены в указанном [списке объектов todoTaskList, обновлены в нем или удалены из него.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="f4766-105">Get a set of [todoTask](../resources/todotask.md) resources that have been added, deleted, or updated in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

<span data-ttu-id="f4766-106">Вызов **функции delta** **для ресурсов todoTask** в **todoTaskList** аналогичен запросу GET, за исключением того, что корректно применяя [маркеры состояния](/graph/delta-query-overview) в одном или нескольких из этих вызовов, вы можете запросить добавочные изменения в **todoTask** **list.**</span><span class="sxs-lookup"><span data-stu-id="f4766-106">A **delta** function call for **todoTask** resources in a **todoTaskList** is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the **todoTask** in that **todoTaskList**.</span></span> <span data-ttu-id="f4766-107">Это позволяет поддерживать и синхронизировать локальное хранилище **ресурсов todoTask** пользователя, не каждый раз берет весь набор с сервера.</span><span class="sxs-lookup"><span data-stu-id="f4766-107">This allows you to maintain and synchronize a local store of a user's **todoTask** resources without having to fetch the entire set from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="f4766-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4766-108">Permissions</span></span>
<span data-ttu-id="f4766-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4766-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4766-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4766-111">Permission type</span></span>      | <span data-ttu-id="f4766-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4766-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4766-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4766-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f4766-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4766-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f4766-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4766-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4766-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4766-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f4766-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4766-117">Application</span></span> | <span data-ttu-id="f4766-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f4766-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4766-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4766-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/{id}/tasks/delta
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/delta
```

## <a name="query-parameters"></a><span data-ttu-id="f4766-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f4766-120">Query parameters</span></span>

<span data-ttu-id="f4766-121">Отслеживание изменений в **коллекции todoTask** влечет за ни один или **несколько дельта-функций.**</span><span class="sxs-lookup"><span data-stu-id="f4766-121">Tracking changes in a **todoTask** collection incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="f4766-122">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="f4766-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="f4766-123">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="f4766-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="f4766-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="f4766-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="f4766-125">В последующих запросах просто скопируйте и примените `nextLink` `deltaLink` или введите URL-адрес из предыдущего ответа, так как в нем уже содержатся закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="f4766-125">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f4766-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="f4766-126">Query parameter</span></span>      | <span data-ttu-id="f4766-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f4766-127">Type</span></span>   |<span data-ttu-id="f4766-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f4766-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4766-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f4766-129">$deltatoken</span></span> | <span data-ttu-id="f4766-130">string</span><span class="sxs-lookup"><span data-stu-id="f4766-130">string</span></span> | <span data-ttu-id="f4766-131">Маркер [состояния, возвращенный](/graph/delta-query-overview) в `deltaLink` URL-адресе предыдущего **вызова функции delta** для той же коллекции todoTask и указывает на завершение этого цикла отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="f4766-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same todoTask collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="f4766-132">Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="f4766-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f4766-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f4766-133">$skiptoken</span></span> | <span data-ttu-id="f4766-134">строка</span><span class="sxs-lookup"><span data-stu-id="f4766-134">string</span></span> | <span data-ttu-id="f4766-135">Маркер [состояния, возвращаемый](/graph/delta-query-overview) в `nextLink` URL-адресе предыдущего вызова **функции delta** и указывающий, что в той же коллекции todoTask остаются не все изменения.</span><span class="sxs-lookup"><span data-stu-id="f4766-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same todoTask collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="f4766-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="f4766-136">OData query parameters</span></span>

- <span data-ttu-id="f4766-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="f4766-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="f4766-139">Поддержка запросов `$select` `$top` изменений, и `$expand` для todoTask.</span><span class="sxs-lookup"><span data-stu-id="f4766-139">Delta query support `$select`, `$top`, and `$expand` for todoTask.</span></span> 
- <span data-ttu-id="f4766-140">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="f4766-140">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="f4766-141">Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="f4766-141">The only supported `$filter` expressions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="f4766-p106">Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="f4766-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="f4766-144">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4766-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4766-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4766-145">Request headers</span></span>
| <span data-ttu-id="f4766-146">Имя</span><span class="sxs-lookup"><span data-stu-id="f4766-146">Name</span></span>       | <span data-ttu-id="f4766-147">Тип</span><span class="sxs-lookup"><span data-stu-id="f4766-147">Type</span></span> | <span data-ttu-id="f4766-148">Описание</span><span class="sxs-lookup"><span data-stu-id="f4766-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="f4766-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4766-149">Authorization</span></span>  | <span data-ttu-id="f4766-150">string</span><span class="sxs-lookup"><span data-stu-id="f4766-150">string</span></span>  | <span data-ttu-id="f4766-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4766-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4766-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4766-153">Content-Type</span></span>  | <span data-ttu-id="f4766-154">string</span><span class="sxs-lookup"><span data-stu-id="f4766-154">string</span></span>  | <span data-ttu-id="f4766-p108">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4766-p108">application/json. Required.</span></span> |
| <span data-ttu-id="f4766-157">Prefer</span><span class="sxs-lookup"><span data-stu-id="f4766-157">Prefer</span></span> | <span data-ttu-id="f4766-158">string</span><span class="sxs-lookup"><span data-stu-id="f4766-158">string</span></span>  | <span data-ttu-id="f4766-p109">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f4766-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f4766-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4766-161">Response</span></span>

<span data-ttu-id="f4766-162">При успешном выполнении этот метод возвращает `200 OK` код отклика [и объект коллекции todoTask](../resources/todotask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4766-162">If successful, this method returns a `200 OK` response code and [todoTask](../resources/todotask.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4766-163">Пример</span><span class="sxs-lookup"><span data-stu-id="f4766-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4766-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4766-164">Request</span></span>
<span data-ttu-id="f4766-165">В следующем примере показано, как выполнить один **вызов функции delta** и ограничить максимальное количество **ресурсов todoTask** в теле отклика до 2.</span><span class="sxs-lookup"><span data-stu-id="f4766-165">The following example shows how to make a single **delta** function call, and limit the maximum number of **todoTask** in the response body to 2.</span></span>

<span data-ttu-id="f4766-166">Чтобы отследить изменения **в ресурсах todoTask** **в todoTaskList,** выполните один или несколько вызовов функции **delta,** чтобы получить набор добавочных изменений с момента последнего разностного запроса.</span><span class="sxs-lookup"><span data-stu-id="f4766-166">To track changes in the **todoTask** resources in a **todoTaskList**, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query.</span></span> 
 

### <a name="http-request"></a><span data-ttu-id="f4766-167">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4766-167">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
Prefer: odata.maxpagesize=2
```


### <a name="response"></a><span data-ttu-id="f4766-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4766-168">Response</span></span>
<span data-ttu-id="f4766-169">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="f4766-169">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="f4766-p110">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="f4766-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="f4766-172">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="f4766-172">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="f4766-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4766-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
  "value": [
         "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ9xQ==\"",
         "importance":"normal",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"empty task3",
         "createdDateTime":"2020-08-12T04:54:29.1925206Z",
         "lastModifiedDateTime":"2020-08-12T04:54:29.4903939Z",
         "id":"AAMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZDEwMwBGAAAAAAB5M0K0qlJySLOAgV22zPnuBwDit9FUg_L0SpeANtzxTscbAAMNmhwmAADit9FUg_L0SpeANtzxTscbAAMxlnrYAAA=",
         "body":{
            "content":"",
            "contentType":"text"
         }
      },
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="f4766-175">См. также</span><span class="sxs-lookup"><span data-stu-id="f4766-175">See also</span></span>

- [<span data-ttu-id="f4766-176">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f4766-176">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)