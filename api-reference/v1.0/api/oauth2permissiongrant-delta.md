---
title: 'oauth2permissiongrant: Delta'
description: Получите только что созданный, обновленный или удаленный oauth2permissiongrants, не выполняя полный просмотр всей коллекции ресурсов.
localization_priority: Normal
author: psignoret
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e2c4a4217a00dfa43f256c6896868909e4223f1d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509856"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="44363-103">oauth2permissiongrant: Delta</span><span class="sxs-lookup"><span data-stu-id="44363-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="44363-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44363-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44363-105">Получение только что созданных, обновленных или удаленных объектов [oauth2permissiongrant](../resources/oauth2permissiongrant.md) без выполнения полного считывания всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="44363-105">Get newly created, updated, or deleted [oauth2permissiongrant](../resources/oauth2permissiongrant.md) objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="44363-106">Подробнее: [Использование запроса изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="44363-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="44363-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44363-107">Permissions</span></span>

<span data-ttu-id="44363-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44363-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="44363-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44363-110">Permission type</span></span>      | <span data-ttu-id="44363-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44363-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44363-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44363-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44363-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44363-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44363-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44363-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44363-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44363-115">Not supported.</span></span>    |
|<span data-ttu-id="44363-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="44363-116">oauth2permissiongrant</span></span> | <span data-ttu-id="44363-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44363-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44363-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44363-118">HTTP request</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2permissiongrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="44363-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="44363-119">Query parameters</span></span>

<span data-ttu-id="44363-120">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="44363-120">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="44363-121">Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**.</span><span class="sxs-lookup"><span data-stu-id="44363-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="44363-122">Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.</span><span class="sxs-lookup"><span data-stu-id="44363-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="44363-123">Параметры запроса необходимо указывать только один раз.</span><span class="sxs-lookup"><span data-stu-id="44363-123">You only need to specify query parameters once.</span></span> <span data-ttu-id="44363-124">В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа.</span><span class="sxs-lookup"><span data-stu-id="44363-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="44363-125">URL-адрес содержит закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="44363-125">The URL includes the encoded parameters.</span></span>

| <span data-ttu-id="44363-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="44363-126">Query parameter</span></span>      | <span data-ttu-id="44363-127">Тип</span><span class="sxs-lookup"><span data-stu-id="44363-127">Type</span></span>   |<span data-ttu-id="44363-128">Описание</span><span class="sxs-lookup"><span data-stu-id="44363-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="44363-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="44363-129">$deltatoken</span></span> | <span data-ttu-id="44363-130">string</span><span class="sxs-lookup"><span data-stu-id="44363-130">string</span></span> | <span data-ttu-id="44363-131">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="44363-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="44363-132">Сохраните и примените весь `deltaLink` URL-адрес, включая этот маркер, в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="44363-132">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="44363-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="44363-133">$skiptoken</span></span> | <span data-ttu-id="44363-134">string</span><span class="sxs-lookup"><span data-stu-id="44363-134">string</span></span> | <span data-ttu-id="44363-135">[Маркер состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая на то, что в коллекции ресурсов имеются дальнейшие изменения, которые необходимо отслеживать.</span><span class="sxs-lookup"><span data-stu-id="44363-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="44363-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="44363-136">Optional query parameters</span></span>

<span data-ttu-id="44363-137">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="44363-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="44363-138">`$select`С помощью параметра запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="44363-138">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="44363-139">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="44363-139">The **id** property is always returned.</span></span>
- <span data-ttu-id="44363-140">`$filter`Параметр Query можно использовать только для отслеживания изменений определенных ресурсов с помощью идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="44363-140">The `$filter` query parameter can only be used to track changes on specific resources by using the resource ID.</span></span> <span data-ttu-id="44363-141">Например, `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="44363-141">For example, `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="44363-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44363-142">Request headers</span></span>
| <span data-ttu-id="44363-143">Имя</span><span class="sxs-lookup"><span data-stu-id="44363-143">Name</span></span>       | <span data-ttu-id="44363-144">Описание</span><span class="sxs-lookup"><span data-stu-id="44363-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44363-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44363-145">Authorization</span></span>  | <span data-ttu-id="44363-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44363-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44363-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44363-148">Request body</span></span>
<span data-ttu-id="44363-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44363-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44363-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="44363-150">Response</span></span>

<span data-ttu-id="44363-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [oauth2permissiongrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44363-151">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="44363-152">Оклик также содержит URL-адрес `nextLink` или `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="44363-152">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="44363-153">Если `nextLink` возвращается URL-адрес, дополнительные страницы данных можно получить в сеансе.</span><span class="sxs-lookup"><span data-stu-id="44363-153">If a `nextLink` URL is returned, additional pages of data can be retrieved in the session.</span></span> <span data-ttu-id="44363-154">**Oauth2permissiongrant** продолжает совершать запросы, используя `nextLink` URL-адрес, пока `deltaLink` в ответ не будет включен URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="44363-154">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="44363-155">Если `deltaLink` возвращается URL-адрес, дополнительные данные о ресурсе не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="44363-155">If a `deltaLink` URL is returned, no more data about the resource is returned.</span></span> <span data-ttu-id="44363-156">Следует оставить и использовать `deltaLink` URL-адрес для получения сведений об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="44363-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="44363-157">Подробнее: [Использование запроса изменений](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="44363-157">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="44363-158">Примеры запросов приведены в статье [получение добавочных изменений для пользователей](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="44363-158">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="44363-159">Пример</span><span class="sxs-lookup"><span data-stu-id="44363-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="44363-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="44363-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="44363-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="44363-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta
```
# <a name="c"></a>[<span data-ttu-id="44363-162">C#</span><span class="sxs-lookup"><span data-stu-id="44363-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44363-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44363-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44363-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44363-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44363-165">Java</span><span class="sxs-lookup"><span data-stu-id="44363-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="44363-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="44363-166">Response</span></span>
><span data-ttu-id="44363-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44363-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
