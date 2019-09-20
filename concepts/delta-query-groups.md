---
title: Получение добавочных изменений для групп
description: Разностный запрос позволяет запрашивать добавления, удаления или обновления групп с помощью разностных вызовов функций. Разностный запрос позволяет находить изменения в группах
author: piotrci
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: fac0aaf0e895c0bdd44434174cf2cc24b99fd5c6
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053923"
---
# <a name="get-incremental-changes-for-groups"></a><span data-ttu-id="0317f-104">Получение добавочных изменений для групп</span><span class="sxs-lookup"><span data-stu-id="0317f-104">Get incremental changes for groups</span></span>

<span data-ttu-id="0317f-p102">[Запрос изменений](./delta-query-overview.md) позволяет запрашивать добавления, удаления или обновления групп с помощью серии вызовов функции [delta](/graph/api/group-delta?view=graph-rest-1.0). Запрос изменений позволяет находить изменения в группах. При этом не требуется получать полный набор групп из Microsoft Graph и сравнивать изменения.</span><span class="sxs-lookup"><span data-stu-id="0317f-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to groups, by way of a series of [delta](/graph/api/group-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to groups without having to fetch the entire set of groups from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="0317f-p103">Клиенты, выполняющие синхронизацию групп с локальным хранилищем профилей, в ближайшем будущем смогут использовать запрос изменений как для первичной полной синхронизации, так и для добавочной синхронизации. Как правило, сначала выполняется полная синхронизация групп в клиенте, а затем в группы периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="0317f-p103">Clients using synchronizing groups with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the groups in a tenant, and subsequently, get incremental changes to groups periodically.</span></span>

## <a name="tracking-group-changes"></a><span data-ttu-id="0317f-109">Отслеживание изменений в группах</span><span class="sxs-lookup"><span data-stu-id="0317f-109">Tracking group changes</span></span>

<span data-ttu-id="0317f-p104">Как правило, цикл отслеживания изменений в группах состоит из одного или нескольких запросов GET с функцией **delta**. Запрос GET совершается практически так же, как и при [получении списка групп](/graph/api/group-list?view=graph-rest-1.0), но в него нужно включить:</span><span class="sxs-lookup"><span data-stu-id="0317f-p104">Tracking group changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list groups](/graph/api/group-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="0317f-112">функцию **delta**;</span><span class="sxs-lookup"><span data-stu-id="0317f-112">The **delta** function.</span></span>
- <span data-ttu-id="0317f-113">[маркер состояния](./delta-query-overview.md) (*deltaToken* или *skipToken*) из данных предыдущего вызова функции **delta** в запросе GET.</span><span class="sxs-lookup"><span data-stu-id="0317f-113">A [state token](./delta-query-overview.md) (*deltaToken* or *skipToken*) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="0317f-114">Пример</span><span class="sxs-lookup"><span data-stu-id="0317f-114">Example</span></span>

<span data-ttu-id="0317f-115">В следующем примере показана серия запросов для отслеживания изменений в группах:</span><span class="sxs-lookup"><span data-stu-id="0317f-115">The following example shows a series  requests to track changes to groups:</span></span>

1. <span data-ttu-id="0317f-116">[Исходный запрос](#initial-request) и [ответ](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="0317f-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="0317f-117">[Запрос nextLink](#nextlink-request) и [ответ](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="0317f-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="0317f-118">[Последний запрос nextLink](#final-nextlink-request) и [ответ](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="0317f-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="0317f-119">[Запрос deltaLink ](#deltalink-request) и [ответ deltaLink](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="0317f-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="0317f-120">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="0317f-120">Initial request</span></span>

<span data-ttu-id="0317f-121">Чтобы начать отслеживать изменения в ресурсе группы, необходимо совершить к нему запрос, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="0317f-121">To begin tracking changes in the group resource, you make a request including the delta function on the group resource.</span></span>

<span data-ttu-id="0317f-122">Обратите внимание на следующее:</span><span class="sxs-lookup"><span data-stu-id="0317f-122">Note the following:</span></span>

- <span data-ttu-id="0317f-123">Необязательный параметр `$select` включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.</span><span class="sxs-lookup"><span data-stu-id="0317f-123">The optional `$select` query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="0317f-124">Необязательный параметр `$expand` включен в запрос, чтобы показать, как членов групп можно получать вместе с объектами групп.</span><span class="sxs-lookup"><span data-stu-id="0317f-124">The optional `$expand` query parameter is included to show how group members can be retrieved together with group objects.</span></span> <span data-ttu-id="0317f-125">Это позволяет отслеживать изменения членства, например добавление или удаление пользователей из групп.</span><span class="sxs-lookup"><span data-stu-id="0317f-125">This allows tracking of membership changes, such as when users are added or removed from groups.</span></span>
- <span data-ttu-id="0317f-p106">Исходный запрос не включает маркер состояния. Маркеры состояния будут использоваться в последующих запросах.</span><span class="sxs-lookup"><span data-stu-id="0317f-p106">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

## <a name="initial-response"></a><span data-ttu-id="0317f-128">Исходный отклик</span><span class="sxs-lookup"><span data-stu-id="0317f-128">Initial response</span></span>

<span data-ttu-id="0317f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](/graph/api/resources/group?view=graph-rest-1.0) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0317f-129">If successful, this method returns `200 OK` response code and [group](/graph/api/resources/group?view=graph-rest-1.0) collection object in the response body.</span></span> <span data-ttu-id="0317f-130">Если весь набор групп не помещается в один отклик, также будет включена ссылка `nextLink`, содержащая маркер состояния.</span><span class="sxs-lookup"><span data-stu-id="0317f-130">If the entire set of groups is too large to fit in one response, a `nextLink` containing a state token will also be included.</span></span>

<span data-ttu-id="0317f-131">В этом примере в запрос включена ссылка `nextLink`. Исходные параметры `$select` и `$expand` закодированы в маркере состояния.</span><span class="sxs-lookup"><span data-stu-id="0317f-131">In this example, a `nextLink` was included; the original `$select` and `$expand` query parameters are encoded in the state token.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

><span data-ttu-id="0317f-132">**Примечание:** свойство `members@delta` включено в первый объект группы — TestGroup1 — и содержит двух текущих членов группы.</span><span class="sxs-lookup"><span data-stu-id="0317f-132">**Note:** The `members@delta` property is included in the first group object - TestGroup1 - and contains the two current members of the group.</span></span> <span data-ttu-id="0317f-133">В объекте TestGroup2 отсутствует это свойство, так как в группе нет участников.</span><span class="sxs-lookup"><span data-stu-id="0317f-133">TestGroup2 does not contain that property because the group does not have any members.</span></span>

## <a name="nextlink-request"></a><span data-ttu-id="0317f-134">Запрос nextLink</span><span class="sxs-lookup"><span data-stu-id="0317f-134">nextLink request</span></span>

<span data-ttu-id="0317f-135">Во втором запросе используется ссылка `nextLink` из предыдущего запроса, содержащая маркер `skipToken`.</span><span class="sxs-lookup"><span data-stu-id="0317f-135">The second request uses the `nextLink` from the previous response, which contains the `skipToken`.</span></span> <span data-ttu-id="0317f-136">Обратите внимание на то, что параметры `$select` и `$expand` не указаны в явном виде, так как они закодированы в маркере.</span><span class="sxs-lookup"><span data-stu-id="0317f-136">Notice the `$select` and `$expand` parameters are not explicitly present as they are encoded in the token.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a><span data-ttu-id="0317f-137">Отклик nextLink</span><span class="sxs-lookup"><span data-stu-id="0317f-137">nextLink response</span></span>

<span data-ttu-id="0317f-138">Отклик содержит ссылку `nextLink` с новым значением `skipToken`, означающим, что доступны дополнительные группы.</span><span class="sxs-lookup"><span data-stu-id="0317f-138">The response contains another `nextLink` with a new `skipToken` value, indicating there are more groups available.</span></span> <span data-ttu-id="0317f-139">Выполнение запросов с использованием URL-адреса `nextLink` должно продолжаться, пока в отклике не будет возвращен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="0317f-139">You continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="0317f-140">Последний запрос nextLink</span><span class="sxs-lookup"><span data-stu-id="0317f-140">Final nextLink request</span></span>

<span data-ttu-id="0317f-141">В третьем запросе снова используется последняя ссылка `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="0317f-141">The third request again uses the latest `nextLink`.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="0317f-142">Последний отклик nextLink</span><span class="sxs-lookup"><span data-stu-id="0317f-142">Final nextLink response</span></span>

<span data-ttu-id="0317f-143">Наконец, возвращается URL-адрес `deltaLink`. Это означает, что больше нет данных о текущем состоянии групп.</span><span class="sxs-lookup"><span data-stu-id="0317f-143">Finally, the `deltaLink` URL is returned, which means there is no more data for the existing state of groups.</span></span> <span data-ttu-id="0317f-144">Для последующих запросов приложение использует ссылку `deltaLink` и содержащееся в ней значение `deltaToken`, чтобы узнавать о новых изменениях групп.</span><span class="sxs-lookup"><span data-stu-id="0317f-144">For future requests, the application uses the `deltaLink` and the `deltaToken` value it contains to learn about new changes to groups.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="0317f-145">Запрос deltaLink</span><span class="sxs-lookup"><span data-stu-id="0317f-145">deltaLink request</span></span>

<span data-ttu-id="0317f-146">С помощью ссылки `deltaLink` из [последнего отклика](#final-nextlink-response) вы сможете получить новые изменения групп с момента последнего запроса.</span><span class="sxs-lookup"><span data-stu-id="0317f-146">Using the `deltaLink` from the [last response](#final-nextlink-response), you will be able to get net new changes to groups since the last request.</span></span> <span data-ttu-id="0317f-147">К таким изменениям относятся:</span><span class="sxs-lookup"><span data-stu-id="0317f-147">Changes include:</span></span>
- <span data-ttu-id="0317f-148">создание объектов групп;</span><span class="sxs-lookup"><span data-stu-id="0317f-148">Newly created group objects.</span></span>
- <span data-ttu-id="0317f-149">удаление объектов групп;</span><span class="sxs-lookup"><span data-stu-id="0317f-149">Deleted group objects.</span></span>
- <span data-ttu-id="0317f-150">изменение свойств объектов групп (например, свойства **displayName**);</span><span class="sxs-lookup"><span data-stu-id="0317f-150">Group objects for which a property has changed (e.g. **displayName** has been modified).</span></span>
- <span data-ttu-id="0317f-151">добавление или удаление объектов членов в объектах групп.</span><span class="sxs-lookup"><span data-stu-id="0317f-151">Group objects for which member objects have been added or removed.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a><span data-ttu-id="0317f-152">Отклик deltaLink</span><span class="sxs-lookup"><span data-stu-id="0317f-152">deltaLink response</span></span>

<span data-ttu-id="0317f-153">Если изменений не произошло, возвращается ссылка `deltaLink` без результатов (свойство `value` остается пустым).</span><span class="sxs-lookup"><span data-stu-id="0317f-153">If no changes have occurred, a `deltaLink` is returned with no results - the `value` property is empty.</span></span> <span data-ttu-id="0317f-154">Обязательно замените предыдущую ссылку в приложении для использования в последующих запросах.</span><span class="sxs-lookup"><span data-stu-id="0317f-154">Make sure to replace the previous link in the application with the new one for use in future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

<span data-ttu-id="0317f-155">Если обнаружены изменения, в отклик включается коллекция измененных групп.</span><span class="sxs-lookup"><span data-stu-id="0317f-155">If changes have occurred, a collection of changed groups is included.</span></span> <span data-ttu-id="0317f-156">Отклик также содержит ссылку `nextLink` (если требуется получить несколько страниц) или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="0317f-156">The response also contains either a `nextLink` - in case there are multiple pages of changes to retrieve - or a `deltaLink`.</span></span> <span data-ttu-id="0317f-157">Следует реализовать такой же порядок перехода по ссылкам `nextLinks`, как и раньше, сохраняя заключительную ссылку `deltaLink` для последующих вызовов.</span><span class="sxs-lookup"><span data-stu-id="0317f-157">You should implement the same pattern of following the `nextLinks` as before and persist the final `deltaLink` for future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```

<span data-ttu-id="0317f-158">Ниже представлены некоторые примечания к приведенному выше примеру отклика.</span><span class="sxs-lookup"><span data-stu-id="0317f-158">Some things to note about the example response above:</span></span>

- <span data-ttu-id="0317f-159">Объекты возвращаются с тем же набором свойств, который изначально указывался с помощью параметров `$select` и `$expand`.</span><span class="sxs-lookup"><span data-stu-id="0317f-159">The objects are returned with the same set of properties originally specified via the `$select` and `$expand` query parameters.</span></span>

- <span data-ttu-id="0317f-160">Включены как измененные, так и оставшиеся без изменений свойства.</span><span class="sxs-lookup"><span data-stu-id="0317f-160">Both changed and unchanged properties are included.</span></span> <span data-ttu-id="0317f-161">В приведенном выше примере свойство `description` содержит новое значение, а свойство `displayName` не изменилось.</span><span class="sxs-lookup"><span data-stu-id="0317f-161">In the example above, the `description` property has a new value, while the `displayName` property has not changed.</span></span>

- <span data-ttu-id="0317f-162">Свойство `members@delta` содержит все изменения членства.</span><span class="sxs-lookup"><span data-stu-id="0317f-162">`members@delta` contains any changes to membership.</span></span>

  - <span data-ttu-id="0317f-163">Первый пользователь в списке был удален из группы путем удаления членства или самого объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="0317f-163">The first user in the list has been removed from the group - either by removing the membership or by deleting the user object itself.</span></span> <span data-ttu-id="0317f-164">Это описывается свойством `@removed`.</span><span class="sxs-lookup"><span data-stu-id="0317f-164">The `@removed` property describes that.</span></span>

  - <span data-ttu-id="0317f-165">Второй пользователь был добавлен в группу.</span><span class="sxs-lookup"><span data-stu-id="0317f-165">The second user has been added to the group.</span></span>

## <a name="paging-through-members-in-a-large-group"></a><span data-ttu-id="0317f-166">Постраничный переход в случае списка членов большой группы</span><span class="sxs-lookup"><span data-stu-id="0317f-166">Paging through members in a large group</span></span>

<span data-ttu-id="0317f-167">Свойство `members@delta` включается в объекты групп по умолчанию, если параметр `$select` не указан в запросе или параметр `$expand=members` указан в явном виде.</span><span class="sxs-lookup"><span data-stu-id="0317f-167">The `members@delta` property is included in group objects by default, when the `$select` query parameter has not been specified, or when the `$expand=members` parameter is explicitly specified.</span></span> <span data-ttu-id="0317f-168">Если в группе много членов, данные о них могут не поместиться в один отклик. В этом разделе описан порядок обработки таких случаев.</span><span class="sxs-lookup"><span data-stu-id="0317f-168">For groups with many members it is possible that all members cannot fit into a single response; in this section we describe the pattern you should implement to handle such cases.</span></span>

><span data-ttu-id="0317f-169">**Примечание.** Этот шаблон применяется как к получению исходного состояния группы, так и к последующим разностным запросам на получение изменений.</span><span class="sxs-lookup"><span data-stu-id="0317f-169">**Note:** This pattern applies to both the initial retrieval of group state as well as to subsequent calls to get delta changes.</span></span>

<span data-ttu-id="0317f-170">Предположим, что выполняется следующий разностный запрос (либо для регистрации полного исходного состояния групп, либо для получения изменений):</span><span class="sxs-lookup"><span data-stu-id="0317f-170">Let's assume you are executing the following delta query - either to capture the initial full state of groups, or later on to get delta changes:</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

1. <span data-ttu-id="0317f-171">Microsoft Graph может вернуть отклик, содержащий только один объект группы с большим списком членов в свойстве `members@delta`:</span><span class="sxs-lookup"><span data-stu-id="0317f-171">Microsoft Graph may return a response that contains just one group object, with a large list of members in the `members@delta` property:</span></span>

<span data-ttu-id="0317f-172">**Первая страница**</span><span class="sxs-lookup"><span data-stu-id="0317f-172">**First page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. <span data-ttu-id="0317f-173">Перейдя по ссылке `nextLink`, вы снова можете получить отклик с таким же объектом группы.</span><span class="sxs-lookup"><span data-stu-id="0317f-173">When you follow the `nextLink` you may receive a response again containing the same group object.</span></span> <span data-ttu-id="0317f-174">Будут возвращены те же значения свойств, но расширенное свойство `members@delta` теперь содержит другой список пользователей.</span><span class="sxs-lookup"><span data-stu-id="0317f-174">The same property values will be returned but the expanded `members@delta` property now contains a different list of users.</span></span>

<span data-ttu-id="0317f-175">**Вторая страница**</span><span class="sxs-lookup"><span data-stu-id="0317f-175">**Second page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. <span data-ttu-id="0317f-176">В конечном итоге будет возвращен весь список членов, и в отклике начнут появляться другие группы.</span><span class="sxs-lookup"><span data-stu-id="0317f-176">Eventually, the entire member list will be returned in this fashion, and other groups will start showing up in the response.</span></span>

<span data-ttu-id="0317f-177">Для корректной реализации этого порядка следуйте приведенным ниже рекомендациям.</span><span class="sxs-lookup"><span data-stu-id="0317f-177">We recommend the following best practices to correctly handle this pattern:</span></span>
- <span data-ttu-id="0317f-178">Всегда переходите по ссылке `nextLink` и локально выполняйте объединение для состояния каждой группы. По мере получения откликов для одной и той же группы составляйте полный список членов в приложении.</span><span class="sxs-lookup"><span data-stu-id="0317f-178">Always follow `nextLink` and locally merge each group's state: as you receive responses related to the same group, use them to build the full membership list in your application.</span></span>
- <span data-ttu-id="0317f-179">Не рекомендуем предполагать, что отклики будут представлены в определенной последовательности.</span><span class="sxs-lookup"><span data-stu-id="0317f-179">It is best not to assume a specific sequence of the responses.</span></span> <span data-ttu-id="0317f-180">Предполагайте, что одна и та же группа может встречаться в любом месте последовательности `nextLink`, и обрабатывайте этот случай в логике объединения.</span><span class="sxs-lookup"><span data-stu-id="0317f-180">Assume that the same group could show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>


## <a name="see-also"></a><span data-ttu-id="0317f-181">См. также</span><span class="sxs-lookup"><span data-stu-id="0317f-181">See also</span></span>
<span data-ttu-id="0317f-182">Обзор [запросов изменений Microsoft Graph](delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="0317f-182">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
