---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653f2fcb01e7fb0db5599b3dbc87fa7f38827ffd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414226"
---
# <a name="update-orgcontact"></a><span data-ttu-id="afc1a-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="afc1a-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afc1a-104">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="afc1a-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="afc1a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afc1a-105">Permissions</span></span>
<span data-ttu-id="afc1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afc1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afc1a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afc1a-108">Permission type</span></span>      | <span data-ttu-id="afc1a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afc1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afc1a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afc1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afc1a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afc1a-111">Not supported.</span></span>    |
|<span data-ttu-id="afc1a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afc1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afc1a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afc1a-113">Not supported.</span></span>    |
|<span data-ttu-id="afc1a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afc1a-114">Application</span></span> | <span data-ttu-id="afc1a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afc1a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afc1a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afc1a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="afc1a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afc1a-117">Request headers</span></span>
| <span data-ttu-id="afc1a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="afc1a-118">Name</span></span>       | <span data-ttu-id="afc1a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="afc1a-119">Type</span></span> | <span data-ttu-id="afc1a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="afc1a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="afc1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="afc1a-121">Authorization</span></span>  | <span data-ttu-id="afc1a-122">string</span><span class="sxs-lookup"><span data-stu-id="afc1a-122">string</span></span>  | <span data-ttu-id="afc1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afc1a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afc1a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="afc1a-125">Request body</span></span>
<span data-ttu-id="afc1a-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="afc1a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="afc1a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="afc1a-129">Property</span></span>     | <span data-ttu-id="afc1a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="afc1a-130">Type</span></span>   |<span data-ttu-id="afc1a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="afc1a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afc1a-132">city</span><span class="sxs-lookup"><span data-stu-id="afc1a-132">city</span></span>|<span data-ttu-id="afc1a-133">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-133">String</span></span>||
|<span data-ttu-id="afc1a-134">country</span><span class="sxs-lookup"><span data-stu-id="afc1a-134">country</span></span>|<span data-ttu-id="afc1a-135">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-135">String</span></span>||
|<span data-ttu-id="afc1a-136">department</span><span class="sxs-lookup"><span data-stu-id="afc1a-136">department</span></span>|<span data-ttu-id="afc1a-137">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-137">String</span></span>||
|<span data-ttu-id="afc1a-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="afc1a-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="afc1a-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="afc1a-139">Boolean</span></span>||
|<span data-ttu-id="afc1a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="afc1a-140">displayName</span></span>|<span data-ttu-id="afc1a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="afc1a-141">String</span></span>||
|<span data-ttu-id="afc1a-142">givenName</span><span class="sxs-lookup"><span data-stu-id="afc1a-142">givenName</span></span>|<span data-ttu-id="afc1a-143">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-143">String</span></span>||
|<span data-ttu-id="afc1a-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="afc1a-144">jobTitle</span></span>|<span data-ttu-id="afc1a-145">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-145">String</span></span>||
|<span data-ttu-id="afc1a-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="afc1a-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="afc1a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afc1a-147">DateTimeOffset</span></span>||
|<span data-ttu-id="afc1a-148">mail</span><span class="sxs-lookup"><span data-stu-id="afc1a-148">mail</span></span>|<span data-ttu-id="afc1a-149">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-149">String</span></span>||
|<span data-ttu-id="afc1a-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="afc1a-150">mailNickname</span></span>|<span data-ttu-id="afc1a-151">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-151">String</span></span>||
|<span data-ttu-id="afc1a-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="afc1a-152">mobilePhone</span></span>|<span data-ttu-id="afc1a-153">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-153">String</span></span>||
|<span data-ttu-id="afc1a-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="afc1a-154">officeLocation</span></span>|<span data-ttu-id="afc1a-155">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-155">String</span></span>||
|<span data-ttu-id="afc1a-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="afc1a-156">postalCode</span></span>|<span data-ttu-id="afc1a-157">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-157">String</span></span>||
|<span data-ttu-id="afc1a-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="afc1a-158">proxyAddresses</span></span>|<span data-ttu-id="afc1a-159">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-159">String</span></span>||
|<span data-ttu-id="afc1a-160">state</span><span class="sxs-lookup"><span data-stu-id="afc1a-160">state</span></span>|<span data-ttu-id="afc1a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="afc1a-161">String</span></span>||
|<span data-ttu-id="afc1a-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="afc1a-162">streetAddress</span></span>|<span data-ttu-id="afc1a-163">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-163">String</span></span>||
|<span data-ttu-id="afc1a-164">surname</span><span class="sxs-lookup"><span data-stu-id="afc1a-164">surname</span></span>|<span data-ttu-id="afc1a-165">String</span><span class="sxs-lookup"><span data-stu-id="afc1a-165">String</span></span>||
|<span data-ttu-id="afc1a-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="afc1a-166">businessPhones</span></span>|<span data-ttu-id="afc1a-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="afc1a-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="afc1a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="afc1a-168">Response</span></span>

<span data-ttu-id="afc1a-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afc1a-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afc1a-170">Пример</span><span class="sxs-lookup"><span data-stu-id="afc1a-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afc1a-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="afc1a-171">Request</span></span>
<span data-ttu-id="afc1a-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afc1a-172">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="afc1a-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="afc1a-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="afc1a-174">C#</span><span class="sxs-lookup"><span data-stu-id="afc1a-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afc1a-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afc1a-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="afc1a-176">Цель — C</span><span class="sxs-lookup"><span data-stu-id="afc1a-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="afc1a-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="afc1a-177">Response</span></span>
<span data-ttu-id="afc1a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afc1a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
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
