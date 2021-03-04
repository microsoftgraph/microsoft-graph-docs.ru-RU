---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 85b08d815b742a0b4117c7dd0ae786da979f92dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447831"
---
# <a name="update-orgcontact"></a><span data-ttu-id="c2039-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="c2039-103">Update orgcontact</span></span>

<span data-ttu-id="c2039-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2039-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2039-105">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="c2039-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2039-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2039-106">Permissions</span></span>
<span data-ttu-id="c2039-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2039-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2039-109">Permission type</span></span>      | <span data-ttu-id="c2039-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2039-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2039-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2039-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2039-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2039-112">Not supported.</span></span>    |
|<span data-ttu-id="c2039-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2039-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2039-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2039-114">Not supported.</span></span>    |
|<span data-ttu-id="c2039-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2039-115">Application</span></span> | <span data-ttu-id="c2039-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2039-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2039-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2039-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c2039-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2039-118">Request headers</span></span>
| <span data-ttu-id="c2039-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c2039-119">Name</span></span>       | <span data-ttu-id="c2039-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c2039-120">Type</span></span> | <span data-ttu-id="c2039-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c2039-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c2039-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2039-122">Authorization</span></span>  | <span data-ttu-id="c2039-123">string</span><span class="sxs-lookup"><span data-stu-id="c2039-123">string</span></span>  | <span data-ttu-id="c2039-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2039-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2039-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2039-126">Request body</span></span>
<span data-ttu-id="c2039-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c2039-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2039-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2039-130">Property</span></span>     | <span data-ttu-id="c2039-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2039-131">Type</span></span>   |<span data-ttu-id="c2039-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2039-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2039-133">city</span><span class="sxs-lookup"><span data-stu-id="c2039-133">city</span></span>|<span data-ttu-id="c2039-134">String</span><span class="sxs-lookup"><span data-stu-id="c2039-134">String</span></span>||
|<span data-ttu-id="c2039-135">country</span><span class="sxs-lookup"><span data-stu-id="c2039-135">country</span></span>|<span data-ttu-id="c2039-136">String</span><span class="sxs-lookup"><span data-stu-id="c2039-136">String</span></span>||
|<span data-ttu-id="c2039-137">department</span><span class="sxs-lookup"><span data-stu-id="c2039-137">department</span></span>|<span data-ttu-id="c2039-138">String</span><span class="sxs-lookup"><span data-stu-id="c2039-138">String</span></span>||
|<span data-ttu-id="c2039-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="c2039-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="c2039-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2039-140">Boolean</span></span>||
|<span data-ttu-id="c2039-141">displayName</span><span class="sxs-lookup"><span data-stu-id="c2039-141">displayName</span></span>|<span data-ttu-id="c2039-142">String</span><span class="sxs-lookup"><span data-stu-id="c2039-142">String</span></span>||
|<span data-ttu-id="c2039-143">givenName</span><span class="sxs-lookup"><span data-stu-id="c2039-143">givenName</span></span>|<span data-ttu-id="c2039-144">String</span><span class="sxs-lookup"><span data-stu-id="c2039-144">String</span></span>||
|<span data-ttu-id="c2039-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c2039-145">jobTitle</span></span>|<span data-ttu-id="c2039-146">String</span><span class="sxs-lookup"><span data-stu-id="c2039-146">String</span></span>||
|<span data-ttu-id="c2039-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c2039-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="c2039-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2039-148">DateTimeOffset</span></span>||
|<span data-ttu-id="c2039-149">почта;</span><span class="sxs-lookup"><span data-stu-id="c2039-149">mail</span></span>|<span data-ttu-id="c2039-150">String</span><span class="sxs-lookup"><span data-stu-id="c2039-150">String</span></span>||
|<span data-ttu-id="c2039-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c2039-151">mailNickname</span></span>|<span data-ttu-id="c2039-152">String</span><span class="sxs-lookup"><span data-stu-id="c2039-152">String</span></span>||
|<span data-ttu-id="c2039-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c2039-153">mobilePhone</span></span>|<span data-ttu-id="c2039-154">String</span><span class="sxs-lookup"><span data-stu-id="c2039-154">String</span></span>||
|<span data-ttu-id="c2039-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c2039-155">officeLocation</span></span>|<span data-ttu-id="c2039-156">String</span><span class="sxs-lookup"><span data-stu-id="c2039-156">String</span></span>||
|<span data-ttu-id="c2039-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="c2039-157">postalCode</span></span>|<span data-ttu-id="c2039-158">String</span><span class="sxs-lookup"><span data-stu-id="c2039-158">String</span></span>||
|<span data-ttu-id="c2039-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="c2039-159">proxyAddresses</span></span>|<span data-ttu-id="c2039-160">String</span><span class="sxs-lookup"><span data-stu-id="c2039-160">String</span></span>||
|<span data-ttu-id="c2039-161">state</span><span class="sxs-lookup"><span data-stu-id="c2039-161">state</span></span>|<span data-ttu-id="c2039-162">String</span><span class="sxs-lookup"><span data-stu-id="c2039-162">String</span></span>||
|<span data-ttu-id="c2039-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="c2039-163">streetAddress</span></span>|<span data-ttu-id="c2039-164">String</span><span class="sxs-lookup"><span data-stu-id="c2039-164">String</span></span>||
|<span data-ttu-id="c2039-165">surname</span><span class="sxs-lookup"><span data-stu-id="c2039-165">surname</span></span>|<span data-ttu-id="c2039-166">String</span><span class="sxs-lookup"><span data-stu-id="c2039-166">String</span></span>||
|<span data-ttu-id="c2039-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="c2039-167">businessPhones</span></span>|<span data-ttu-id="c2039-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2039-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="c2039-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2039-169">Response</span></span>

<span data-ttu-id="c2039-170">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2039-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2039-171">Пример</span><span class="sxs-lookup"><span data-stu-id="c2039-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2039-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2039-172">Request</span></span>
<span data-ttu-id="c2039-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2039-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2039-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2039-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c2039-175">C#</span><span class="sxs-lookup"><span data-stu-id="c2039-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2039-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2039-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2039-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2039-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c2039-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2039-178">Response</span></span>
<span data-ttu-id="c2039-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2039-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


