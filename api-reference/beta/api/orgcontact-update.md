---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c425af3a39a2a9f13a46792d8482d59804c8d37f
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352158"
---
# <a name="update-orgcontact"></a><span data-ttu-id="72df1-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="72df1-103">Update orgcontact</span></span>

<span data-ttu-id="72df1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72df1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72df1-105">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="72df1-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="72df1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72df1-106">Permissions</span></span>
<span data-ttu-id="72df1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72df1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72df1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72df1-109">Permission type</span></span>      | <span data-ttu-id="72df1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72df1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72df1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72df1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72df1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72df1-112">Not supported.</span></span>    |
|<span data-ttu-id="72df1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72df1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72df1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72df1-114">Not supported.</span></span>    |
|<span data-ttu-id="72df1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72df1-115">Application</span></span> | <span data-ttu-id="72df1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72df1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72df1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72df1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="72df1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72df1-118">Request headers</span></span>
| <span data-ttu-id="72df1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72df1-119">Name</span></span>       | <span data-ttu-id="72df1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="72df1-120">Type</span></span> | <span data-ttu-id="72df1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="72df1-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="72df1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72df1-122">Authorization</span></span>  | <span data-ttu-id="72df1-123">string</span><span class="sxs-lookup"><span data-stu-id="72df1-123">string</span></span>  | <span data-ttu-id="72df1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72df1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72df1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72df1-126">Request body</span></span>
<span data-ttu-id="72df1-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="72df1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="72df1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72df1-130">Property</span></span>     | <span data-ttu-id="72df1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72df1-131">Type</span></span>   |<span data-ttu-id="72df1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72df1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72df1-133">city</span><span class="sxs-lookup"><span data-stu-id="72df1-133">city</span></span>|<span data-ttu-id="72df1-134">String</span><span class="sxs-lookup"><span data-stu-id="72df1-134">String</span></span>||
|<span data-ttu-id="72df1-135">country</span><span class="sxs-lookup"><span data-stu-id="72df1-135">country</span></span>|<span data-ttu-id="72df1-136">Строка</span><span class="sxs-lookup"><span data-stu-id="72df1-136">String</span></span>||
|<span data-ttu-id="72df1-137">department</span><span class="sxs-lookup"><span data-stu-id="72df1-137">department</span></span>|<span data-ttu-id="72df1-138">String</span><span class="sxs-lookup"><span data-stu-id="72df1-138">String</span></span>||
|<span data-ttu-id="72df1-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="72df1-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="72df1-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="72df1-140">Boolean</span></span>||
|<span data-ttu-id="72df1-141">displayName</span><span class="sxs-lookup"><span data-stu-id="72df1-141">displayName</span></span>|<span data-ttu-id="72df1-142">Строка</span><span class="sxs-lookup"><span data-stu-id="72df1-142">String</span></span>||
|<span data-ttu-id="72df1-143">givenName</span><span class="sxs-lookup"><span data-stu-id="72df1-143">givenName</span></span>|<span data-ttu-id="72df1-144">String</span><span class="sxs-lookup"><span data-stu-id="72df1-144">String</span></span>||
|<span data-ttu-id="72df1-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="72df1-145">jobTitle</span></span>|<span data-ttu-id="72df1-146">String</span><span class="sxs-lookup"><span data-stu-id="72df1-146">String</span></span>||
|<span data-ttu-id="72df1-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="72df1-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="72df1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72df1-148">DateTimeOffset</span></span>||
|<span data-ttu-id="72df1-149">mail</span><span class="sxs-lookup"><span data-stu-id="72df1-149">mail</span></span>|<span data-ttu-id="72df1-150">String</span><span class="sxs-lookup"><span data-stu-id="72df1-150">String</span></span>||
|<span data-ttu-id="72df1-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="72df1-151">mailNickname</span></span>|<span data-ttu-id="72df1-152">String</span><span class="sxs-lookup"><span data-stu-id="72df1-152">String</span></span>||
|<span data-ttu-id="72df1-153">mobilePhone;</span><span class="sxs-lookup"><span data-stu-id="72df1-153">mobilePhone</span></span>|<span data-ttu-id="72df1-154">String</span><span class="sxs-lookup"><span data-stu-id="72df1-154">String</span></span>||
|<span data-ttu-id="72df1-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="72df1-155">officeLocation</span></span>|<span data-ttu-id="72df1-156">String</span><span class="sxs-lookup"><span data-stu-id="72df1-156">String</span></span>||
|<span data-ttu-id="72df1-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="72df1-157">postalCode</span></span>|<span data-ttu-id="72df1-158">String</span><span class="sxs-lookup"><span data-stu-id="72df1-158">String</span></span>||
|<span data-ttu-id="72df1-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="72df1-159">proxyAddresses</span></span>|<span data-ttu-id="72df1-160">String</span><span class="sxs-lookup"><span data-stu-id="72df1-160">String</span></span>||
|<span data-ttu-id="72df1-161">state</span><span class="sxs-lookup"><span data-stu-id="72df1-161">state</span></span>|<span data-ttu-id="72df1-162">String</span><span class="sxs-lookup"><span data-stu-id="72df1-162">String</span></span>||
|<span data-ttu-id="72df1-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="72df1-163">streetAddress</span></span>|<span data-ttu-id="72df1-164">String</span><span class="sxs-lookup"><span data-stu-id="72df1-164">String</span></span>||
|<span data-ttu-id="72df1-165">surname</span><span class="sxs-lookup"><span data-stu-id="72df1-165">surname</span></span>|<span data-ttu-id="72df1-166">String</span><span class="sxs-lookup"><span data-stu-id="72df1-166">String</span></span>||
|<span data-ttu-id="72df1-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="72df1-167">businessPhones</span></span>|<span data-ttu-id="72df1-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="72df1-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="72df1-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="72df1-169">Response</span></span>

<span data-ttu-id="72df1-170">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="72df1-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="72df1-171">Пример</span><span class="sxs-lookup"><span data-stu-id="72df1-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72df1-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="72df1-172">Request</span></span>
<span data-ttu-id="72df1-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72df1-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72df1-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="72df1-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="72df1-175">C#</span><span class="sxs-lookup"><span data-stu-id="72df1-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72df1-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72df1-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72df1-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72df1-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="72df1-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="72df1-178">Response</span></span>
<span data-ttu-id="72df1-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72df1-179">The following is an example of the response.</span></span> 
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


