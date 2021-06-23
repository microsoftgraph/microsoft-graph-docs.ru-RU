---
title: Получение добавочных изменений для пользователей
description: Запрос позволяет запрашивать добавления, удаления или обновления пользователей с помощью серии вызовов функции delta. Запрос изменений позволяет находить изменения пользователей. При этом не требуется получать полный набор пользователей из Microsoft Graph и сравнивать изменения.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 39253f03175c9c33c6e358afc2e629a77e449a0c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082064"
---
# <a name="get-incremental-changes-for-users"></a><span data-ttu-id="e1dd9-104">Получение добавочных изменений для пользователей</span><span class="sxs-lookup"><span data-stu-id="e1dd9-104">Get incremental changes for users</span></span>

<span data-ttu-id="e1dd9-p102">[Запрос](./delta-query-overview.md) позволяет запрашивать добавления, удаления или обновления пользователей с помощью серии вызовов функции [delta](/graph/api/user-delta?view=graph-rest-1.0). Запрос изменений позволяет находить изменения пользователей. При этом не требуется получать полный набор пользователей из Microsoft Graph и сравнивать изменения.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to users, by way of a series of [delta](/graph/api/user-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to users without having to fetch the entire set of users from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="e1dd9-p103">Клиенты, выполняющие синхронизацию пользователей с локальным хранилищем профилей, в ближайшем будущем смогут использовать запрос изменений как для первичной полной синхронизации, так и для добавочной синхронизации. Как правило, сначала выполняется полная синхронизация пользователей в клиенте, а потом периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p103">Clients using synchronizing users with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the users in a tenant, and subsequently, get incremental changes to users periodically.</span></span>

## <a name="tracking-user-changes"></a><span data-ttu-id="e1dd9-109">Отслеживание изменений пользователей</span><span class="sxs-lookup"><span data-stu-id="e1dd9-109">Tracking user changes</span></span>

<span data-ttu-id="e1dd9-p104">Как правило, цикл отслеживания изменений пользователей состоит из одного или нескольких запросов GET с вызовом функции **delta**. Запрос GET совершается практически так же, как и при [получении списка пользователей](/graph/api/user-list?view=graph-rest-1.0), но в него нужно включить:</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p104">Tracking user changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list users](/graph/api/user-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="e1dd9-112">функцию **delta**;</span><span class="sxs-lookup"><span data-stu-id="e1dd9-112">The **delta** function.</span></span>
- <span data-ttu-id="e1dd9-113">[маркер состояния](./delta-query-overview.md) (_deltaToken_ или _skipToken_) из данных предыдущего вызова функции **delta** в запросе GET.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-113">A [state token](./delta-query-overview.md) (_deltaToken_ or _skipToken_) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="e1dd9-114">Пример</span><span class="sxs-lookup"><span data-stu-id="e1dd9-114">Example</span></span>

<span data-ttu-id="e1dd9-115">В следующем примере показана серия запросов для отслеживания изменений пользователей:</span><span class="sxs-lookup"><span data-stu-id="e1dd9-115">The following example shows a series  requests to track changes to users:</span></span>

1. <span data-ttu-id="e1dd9-116">[Исходный запрос](#initial-request) и [ответ](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="e1dd9-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="e1dd9-117">[Запрос nextLink](#nextlink-request) и [ответ](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="e1dd9-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="e1dd9-118">[Последний запрос nextLink](#final-nextlink-request) и [ответ](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="e1dd9-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="e1dd9-119">[Запрос deltaLink ](#deltalink-request) и [ответ deltaLink](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="e1dd9-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="e1dd9-120">Исходный запрос</span><span class="sxs-lookup"><span data-stu-id="e1dd9-120">Initial request</span></span>

<span data-ttu-id="e1dd9-121">Чтобы начать отслеживать изменения в ресурсе пользователя, необходимо совершить к нему запрос, включающий функцию delta.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-121">To begin tracking changes in the user resource, you make a request including the delta function on the user resource.</span></span>

<span data-ttu-id="e1dd9-122">Обратите внимание на следующее:</span><span class="sxs-lookup"><span data-stu-id="e1dd9-122">Note the following:</span></span>

- <span data-ttu-id="e1dd9-123">Необязательный параметр $select включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-123">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="e1dd9-p105">Исходный запрос не включает маркер состояния. Маркеры состояния будут использоваться в последующих запросах.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p105">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a><span data-ttu-id="e1dd9-126">Исходный ответ</span><span class="sxs-lookup"><span data-stu-id="e1dd9-126">Initial response</span></span>

<span data-ttu-id="e1dd9-p106">В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](/graph/api/resources/user?view=graph-rest-1.0) в тексте ответа. Если полный набор пользователей не помещается на одну страницу, ответ также будет включать маркер состояния nextLink.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p106">If successful, this method returns `200 OK` response code and [user](/graph/api/resources/user?view=graph-rest-1.0) collection object in the response body. Assuming the entire set of users is too large, the response will also include a nextLink state token.</span></span>

<span data-ttu-id="e1dd9-p107">В этом примере возвращается URL-адрес nextLink. Это означает, что в текущем сеансе можно получить дополнительные страницы данных. Параметр $select из исходного запроса кодируется в URL-адресе nextLink.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p107">In this example, a nextLink URL is returned indicating there are additional pages of data to be retrieved in the session. The $select query parameter from the initial request is encoded into the nextLink URL.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a><span data-ttu-id="e1dd9-131">Запрос nextLink</span><span class="sxs-lookup"><span data-stu-id="e1dd9-131">nextLink request</span></span>

<span data-ttu-id="e1dd9-p108">Второй запрос указывает маркер `skipToken`, полученный из предыдущего ответа. Обратите внимание, что параметр `$select` указывать не обязательно, так как `skipToken` включает его в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p108">The second request specifies the `skipToken` returned from the previous response. Notice the `$select` parameter is not required, as the `skipToken` encodes and includes it.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a><span data-ttu-id="e1dd9-134">Ответ nextLink</span><span class="sxs-lookup"><span data-stu-id="e1dd9-134">nextLink response</span></span>

<span data-ttu-id="e1dd9-135">Ответ содержит ссылку `nextLink` с новым значением `skipToken`, означающим, что доступны дополнительные группы.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-135">The response contains another `nextLink` with a new `skipToken` value, which indicates that more groups are available.</span></span> <span data-ttu-id="e1dd9-136">Вы должны продолжать выполнение запросов с использованием URL-адреса `nextLink`, пока в окончательном ответе не будет возвращен URL-адрес `deltaLink`, даже если значением является пустой массив (это может происходить при некоторых обстоятельствах).</span><span class="sxs-lookup"><span data-stu-id="e1dd9-136">You should continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response, even if the value is an empty array (this can happen under certain circumstances).</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="e1dd9-137">Последний запрос nextLink</span><span class="sxs-lookup"><span data-stu-id="e1dd9-137">Final nextLink request</span></span>

<span data-ttu-id="e1dd9-138">Третий запрос продолжает использовать маркер `skipToken`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-138">The third request continues to use the latest `skipToken` returned from the last sync request.</span></span> 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="e1dd9-139">Последний ответ nextLink</span><span class="sxs-lookup"><span data-stu-id="e1dd9-139">Final nextLink response</span></span>

<span data-ttu-id="e1dd9-p110">Когда возвращается URL-адрес deltaLink, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес deltaLink, чтобы узнавать об изменениях ресурса. Сохраните маркер `deltaToken` и используйте его в URL-адресе запроса, чтобы находить изменения пользователей.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-p110">When the deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource. Save the `deltaToken` and use it in the request URL to discover changes to users.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="e1dd9-143">Запрос deltaLink</span><span class="sxs-lookup"><span data-stu-id="e1dd9-143">deltaLink request</span></span>

<span data-ttu-id="e1dd9-144">С помощью маркера `deltaToken` из [последнего ответа](#final-nextlink-response) вы сможете получить пользователей, измененных (добавленных, удаленных или обновленных) с момента последнего запроса.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-144">Using the `deltaToken` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) users since the last request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a><span data-ttu-id="e1dd9-145">Ответ deltaLink</span><span class="sxs-lookup"><span data-stu-id="e1dd9-145">deltaLink response</span></span>

<span data-ttu-id="e1dd9-146">Если изменений не произошло, возвращается другой маркер `deltatoken` без результатов.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-146">If no changes have occurred, a different `deltatoken` is returned with no results.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

<span data-ttu-id="e1dd9-147">Если же обнаружены изменения, возвращается другой маркер `deltatoken`, включающий коллекцию измененных пользователей.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-147">If changes have occurred, a different `deltatoken` is returned including a collection of changed users.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

<span data-ttu-id="e1dd9-148">Ниже представлены некоторые примечания к предыдущему примеру отклика.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-148">Some things to note about the previous example response:</span></span>

- <span data-ttu-id="e1dd9-149">Если пользователь удален, элемент содержит заметку: `@removed` со значением `"reason": "changed"`.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-149">When the user is deleted, the item contains an annotation: `@removed` with value of `"reason": "changed"`.</span></span>

- <span data-ttu-id="e1dd9-150">Если пользователь удален окончательно, элемент содержит заметку: `@removed` со значением `"reason": "deleted"`.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-150">When the user is permanently deleted, the item contains an annotation: `@removed` with value of `"reason": "deleted"`.</span></span>

- <span data-ttu-id="e1dd9-151">Заметок о создании или восстановлении пользователя не существует.</span><span class="sxs-lookup"><span data-stu-id="e1dd9-151">When the user is created, or restored, there is no annotation.</span></span>

## <a name="see-also"></a><span data-ttu-id="e1dd9-152">См. также</span><span class="sxs-lookup"><span data-stu-id="e1dd9-152">See also</span></span>
<span data-ttu-id="e1dd9-153">Обзор [запросов изменений Microsoft Graph](delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e1dd9-153">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
