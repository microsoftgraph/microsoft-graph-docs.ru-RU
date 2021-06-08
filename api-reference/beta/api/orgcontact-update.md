---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26396518b40023e7a4b5666fb1d00b4effd83546
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785244"
---
# <a name="update-orgcontact"></a><span data-ttu-id="de492-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="de492-103">Update orgcontact</span></span>

<span data-ttu-id="de492-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de492-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de492-105">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="de492-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de492-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de492-106">Permissions</span></span>
<span data-ttu-id="de492-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de492-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de492-109">Permission type</span></span>      | <span data-ttu-id="de492-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de492-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de492-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de492-111">Delegated (work or school account)</span></span> | <span data-ttu-id="de492-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de492-112">Not supported.</span></span>    |
|<span data-ttu-id="de492-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de492-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de492-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de492-114">Not supported.</span></span>    |
|<span data-ttu-id="de492-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de492-115">Application</span></span> | <span data-ttu-id="de492-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de492-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de492-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de492-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="de492-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de492-118">Request headers</span></span>
| <span data-ttu-id="de492-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de492-119">Name</span></span>       | <span data-ttu-id="de492-120">Тип</span><span class="sxs-lookup"><span data-stu-id="de492-120">Type</span></span> | <span data-ttu-id="de492-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de492-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de492-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de492-122">Authorization</span></span>  | <span data-ttu-id="de492-123">string</span><span class="sxs-lookup"><span data-stu-id="de492-123">string</span></span>  | <span data-ttu-id="de492-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de492-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de492-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de492-126">Request body</span></span>
<span data-ttu-id="de492-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="de492-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de492-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de492-130">Property</span></span>     | <span data-ttu-id="de492-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de492-131">Type</span></span>   |<span data-ttu-id="de492-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de492-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de492-133">city</span><span class="sxs-lookup"><span data-stu-id="de492-133">city</span></span>|<span data-ttu-id="de492-134">String</span><span class="sxs-lookup"><span data-stu-id="de492-134">String</span></span>||
|<span data-ttu-id="de492-135">country</span><span class="sxs-lookup"><span data-stu-id="de492-135">country</span></span>|<span data-ttu-id="de492-136">String</span><span class="sxs-lookup"><span data-stu-id="de492-136">String</span></span>||
|<span data-ttu-id="de492-137">department</span><span class="sxs-lookup"><span data-stu-id="de492-137">department</span></span>|<span data-ttu-id="de492-138">String</span><span class="sxs-lookup"><span data-stu-id="de492-138">String</span></span>||
|<span data-ttu-id="de492-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="de492-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="de492-140">Логический</span><span class="sxs-lookup"><span data-stu-id="de492-140">Boolean</span></span>||
|<span data-ttu-id="de492-141">displayName</span><span class="sxs-lookup"><span data-stu-id="de492-141">displayName</span></span>|<span data-ttu-id="de492-142">String</span><span class="sxs-lookup"><span data-stu-id="de492-142">String</span></span>||
|<span data-ttu-id="de492-143">givenName;</span><span class="sxs-lookup"><span data-stu-id="de492-143">givenName</span></span>|<span data-ttu-id="de492-144">String</span><span class="sxs-lookup"><span data-stu-id="de492-144">String</span></span>||
|<span data-ttu-id="de492-145">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="de492-145">jobTitle</span></span>|<span data-ttu-id="de492-146">String</span><span class="sxs-lookup"><span data-stu-id="de492-146">String</span></span>||
|<span data-ttu-id="de492-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="de492-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="de492-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de492-148">DateTimeOffset</span></span>||
|<span data-ttu-id="de492-149">mail</span><span class="sxs-lookup"><span data-stu-id="de492-149">mail</span></span>|<span data-ttu-id="de492-150">String</span><span class="sxs-lookup"><span data-stu-id="de492-150">String</span></span>||
|<span data-ttu-id="de492-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="de492-151">mailNickname</span></span>|<span data-ttu-id="de492-152">String</span><span class="sxs-lookup"><span data-stu-id="de492-152">String</span></span>||
|<span data-ttu-id="de492-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="de492-153">mobilePhone</span></span>|<span data-ttu-id="de492-154">String</span><span class="sxs-lookup"><span data-stu-id="de492-154">String</span></span>||
|<span data-ttu-id="de492-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="de492-155">officeLocation</span></span>|<span data-ttu-id="de492-156">String</span><span class="sxs-lookup"><span data-stu-id="de492-156">String</span></span>||
|<span data-ttu-id="de492-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="de492-157">postalCode</span></span>|<span data-ttu-id="de492-158">String</span><span class="sxs-lookup"><span data-stu-id="de492-158">String</span></span>||
|<span data-ttu-id="de492-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="de492-159">proxyAddresses</span></span>|<span data-ttu-id="de492-160">String</span><span class="sxs-lookup"><span data-stu-id="de492-160">String</span></span>||
|<span data-ttu-id="de492-161">state</span><span class="sxs-lookup"><span data-stu-id="de492-161">state</span></span>|<span data-ttu-id="de492-162">String</span><span class="sxs-lookup"><span data-stu-id="de492-162">String</span></span>||
|<span data-ttu-id="de492-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="de492-163">streetAddress</span></span>|<span data-ttu-id="de492-164">String</span><span class="sxs-lookup"><span data-stu-id="de492-164">String</span></span>||
|<span data-ttu-id="de492-165">surname</span><span class="sxs-lookup"><span data-stu-id="de492-165">surname</span></span>|<span data-ttu-id="de492-166">String</span><span class="sxs-lookup"><span data-stu-id="de492-166">String</span></span>||
|<span data-ttu-id="de492-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="de492-167">businessPhones</span></span>|<span data-ttu-id="de492-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de492-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="de492-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="de492-169">Response</span></span>

<span data-ttu-id="de492-170">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de492-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="de492-171">Пример</span><span class="sxs-lookup"><span data-stu-id="de492-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de492-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="de492-172">Request</span></span>
<span data-ttu-id="de492-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de492-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de492-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="de492-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="de492-175">C#</span><span class="sxs-lookup"><span data-stu-id="de492-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de492-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de492-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de492-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de492-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="de492-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="de492-178">Response</span></span>
<span data-ttu-id="de492-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="de492-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


