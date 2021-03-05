---
title: 'oauth2permissiongrant: дельта'
description: Получить заново созданные, обновленные или удаленные oauth2permissiongrants без выполнения полного чтения всей коллекции ресурсов.
localization_priority: Normal
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 63d936ab649a4e8842d633033a74d8958cd22bed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441783"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="78b6f-103">oauth2permissiongrant: дельта</span><span class="sxs-lookup"><span data-stu-id="78b6f-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="78b6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78b6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78b6f-105">Получить вновь созданные, обновленные или удаленные [объекты oauth2permissiongrant](../resources/oauth2permissiongrant.md) без полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78b6f-105">Get newly created, updated, or deleted [oauth2permissiongrant](../resources/oauth2permissiongrant.md) objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="78b6f-106">Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="78b6f-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="78b6f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78b6f-107">Permissions</span></span>

<span data-ttu-id="78b6f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78b6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="78b6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78b6f-110">Permission type</span></span>      | <span data-ttu-id="78b6f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78b6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78b6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78b6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78b6f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="78b6f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="78b6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78b6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78b6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78b6f-115">Not supported.</span></span>    |
|<span data-ttu-id="78b6f-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="78b6f-116">oauth2permissiongrant</span></span> | <span data-ttu-id="78b6f-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78b6f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78b6f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78b6f-118">HTTP request</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="78b6f-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="78b6f-119">Query parameters</span></span>

<span data-ttu-id="78b6f-120">Отслеживание изменений вызывает один или несколько вызовов функции **дельты.**</span><span class="sxs-lookup"><span data-stu-id="78b6f-120">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="78b6f-121">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="78b6f-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="78b6f-122">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="78b6f-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="78b6f-123">Необходимо указать параметры запроса только один раз.</span><span class="sxs-lookup"><span data-stu-id="78b6f-123">You only need to specify query parameters once.</span></span> <span data-ttu-id="78b6f-124">В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="78b6f-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="78b6f-125">URL-адрес содержит закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="78b6f-125">The URL includes the encoded parameters.</span></span>

| <span data-ttu-id="78b6f-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="78b6f-126">Query parameter</span></span>      | <span data-ttu-id="78b6f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="78b6f-127">Type</span></span>   |<span data-ttu-id="78b6f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="78b6f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78b6f-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="78b6f-129">$deltatoken</span></span> | <span data-ttu-id="78b6f-130">string</span><span class="sxs-lookup"><span data-stu-id="78b6f-130">string</span></span> | <span data-ttu-id="78b6f-131">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений. </span><span class="sxs-lookup"><span data-stu-id="78b6f-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="78b6f-132">Сохраните и примените весь URL-адрес, включая этот маркер, в первом запросе следующего раунда отслеживания `deltaLink` изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="78b6f-132">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="78b6f-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="78b6f-133">$skiptoken</span></span> | <span data-ttu-id="78b6f-134">string</span><span class="sxs-lookup"><span data-stu-id="78b6f-134">string</span></span> | <span data-ttu-id="78b6f-135">Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения. </span><span class="sxs-lookup"><span data-stu-id="78b6f-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="78b6f-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78b6f-136">Optional query parameters</span></span>

<span data-ttu-id="78b6f-137">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="78b6f-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="78b6f-138">Параметр запроса можно указать только свойства, необходимые `$select` для лучшей производительности.</span><span class="sxs-lookup"><span data-stu-id="78b6f-138">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="78b6f-139">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="78b6f-139">The **id** property is always returned.</span></span>
- <span data-ttu-id="78b6f-140">Параметр запроса можно использовать только для отслеживания изменений на определенных `$filter` ресурсах с помощью ИД ресурса.</span><span class="sxs-lookup"><span data-stu-id="78b6f-140">The `$filter` query parameter can only be used to track changes on specific resources by using the resource ID.</span></span> <span data-ttu-id="78b6f-141">Например, `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="78b6f-141">For example, `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="78b6f-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78b6f-142">Request headers</span></span>
| <span data-ttu-id="78b6f-143">Имя</span><span class="sxs-lookup"><span data-stu-id="78b6f-143">Name</span></span>       | <span data-ttu-id="78b6f-144">Описание</span><span class="sxs-lookup"><span data-stu-id="78b6f-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78b6f-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78b6f-145">Authorization</span></span>  | <span data-ttu-id="78b6f-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78b6f-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78b6f-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78b6f-148">Request body</span></span>
<span data-ttu-id="78b6f-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78b6f-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78b6f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="78b6f-150">Response</span></span>

<span data-ttu-id="78b6f-151">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции oauth2permissiongrant](../resources/oauth2permissiongrant.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="78b6f-151">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="78b6f-152">Отклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="78b6f-152">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="78b6f-153">Если URL-адрес возвращается, в сеансе могут быть извлечены `nextLink` дополнительные страницы данных.</span><span class="sxs-lookup"><span data-stu-id="78b6f-153">If a `nextLink` URL is returned, additional pages of data can be retrieved in the session.</span></span> <span data-ttu-id="78b6f-154">**Oauth2permissiongrant** продолжает делать запросы с помощью URL-адреса до тех пор, пока URL-адрес не будет включен `nextLink` `deltaLink` в ответ.</span><span class="sxs-lookup"><span data-stu-id="78b6f-154">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="78b6f-155">Если `deltaLink` URL-адрес возвращается, больше не возвращаются данные о ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78b6f-155">If a `deltaLink` URL is returned, no more data about the resource is returned.</span></span> <span data-ttu-id="78b6f-156">Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="78b6f-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="78b6f-157">Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="78b6f-157">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="78b6f-158">Например, запросы см. [в рублях Получить дополнительные изменения для пользователей.](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="78b6f-158">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="78b6f-159">Пример</span><span class="sxs-lookup"><span data-stu-id="78b6f-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="78b6f-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="78b6f-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="78b6f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="78b6f-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/delta
```
# <a name="c"></a>[<span data-ttu-id="78b6f-162">C#</span><span class="sxs-lookup"><span data-stu-id="78b6f-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78b6f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78b6f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78b6f-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78b6f-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78b6f-165">Java</span><span class="sxs-lookup"><span data-stu-id="78b6f-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="78b6f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="78b6f-166">Response</span></span>
><span data-ttu-id="78b6f-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78b6f-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

