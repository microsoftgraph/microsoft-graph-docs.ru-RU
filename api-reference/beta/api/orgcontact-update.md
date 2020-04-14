---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa9704c44dc8dc7068bf387b97669e2c42aecdd2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403226"
---
# <a name="update-orgcontact"></a><span data-ttu-id="7032c-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="7032c-103">Update orgcontact</span></span>

<span data-ttu-id="7032c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7032c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7032c-105">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="7032c-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7032c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7032c-106">Permissions</span></span>
<span data-ttu-id="7032c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7032c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7032c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7032c-109">Permission type</span></span>      | <span data-ttu-id="7032c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7032c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7032c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7032c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7032c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7032c-112">Not supported.</span></span>    |
|<span data-ttu-id="7032c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7032c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7032c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7032c-114">Not supported.</span></span>    |
|<span data-ttu-id="7032c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7032c-115">Application</span></span> | <span data-ttu-id="7032c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7032c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7032c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7032c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7032c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7032c-118">Request headers</span></span>
| <span data-ttu-id="7032c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7032c-119">Name</span></span>       | <span data-ttu-id="7032c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7032c-120">Type</span></span> | <span data-ttu-id="7032c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7032c-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7032c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7032c-122">Authorization</span></span>  | <span data-ttu-id="7032c-123">string</span><span class="sxs-lookup"><span data-stu-id="7032c-123">string</span></span>  | <span data-ttu-id="7032c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7032c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7032c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7032c-126">Request body</span></span>
<span data-ttu-id="7032c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7032c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7032c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7032c-130">Property</span></span>     | <span data-ttu-id="7032c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7032c-131">Type</span></span>   |<span data-ttu-id="7032c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7032c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7032c-133">city</span><span class="sxs-lookup"><span data-stu-id="7032c-133">city</span></span>|<span data-ttu-id="7032c-134">String</span><span class="sxs-lookup"><span data-stu-id="7032c-134">String</span></span>||
|<span data-ttu-id="7032c-135">country</span><span class="sxs-lookup"><span data-stu-id="7032c-135">country</span></span>|<span data-ttu-id="7032c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="7032c-136">String</span></span>||
|<span data-ttu-id="7032c-137">department</span><span class="sxs-lookup"><span data-stu-id="7032c-137">department</span></span>|<span data-ttu-id="7032c-138">String</span><span class="sxs-lookup"><span data-stu-id="7032c-138">String</span></span>||
|<span data-ttu-id="7032c-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="7032c-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="7032c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="7032c-140">Boolean</span></span>||
|<span data-ttu-id="7032c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7032c-141">displayName</span></span>|<span data-ttu-id="7032c-142">String</span><span class="sxs-lookup"><span data-stu-id="7032c-142">String</span></span>||
|<span data-ttu-id="7032c-143">givenName</span><span class="sxs-lookup"><span data-stu-id="7032c-143">givenName</span></span>|<span data-ttu-id="7032c-144">String</span><span class="sxs-lookup"><span data-stu-id="7032c-144">String</span></span>||
|<span data-ttu-id="7032c-145">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="7032c-145">jobTitle</span></span>|<span data-ttu-id="7032c-146">String</span><span class="sxs-lookup"><span data-stu-id="7032c-146">String</span></span>||
|<span data-ttu-id="7032c-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7032c-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="7032c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7032c-148">DateTimeOffset</span></span>||
|<span data-ttu-id="7032c-149">mail</span><span class="sxs-lookup"><span data-stu-id="7032c-149">mail</span></span>|<span data-ttu-id="7032c-150">String</span><span class="sxs-lookup"><span data-stu-id="7032c-150">String</span></span>||
|<span data-ttu-id="7032c-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7032c-151">mailNickname</span></span>|<span data-ttu-id="7032c-152">String</span><span class="sxs-lookup"><span data-stu-id="7032c-152">String</span></span>||
|<span data-ttu-id="7032c-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="7032c-153">mobilePhone</span></span>|<span data-ttu-id="7032c-154">String</span><span class="sxs-lookup"><span data-stu-id="7032c-154">String</span></span>||
|<span data-ttu-id="7032c-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7032c-155">officeLocation</span></span>|<span data-ttu-id="7032c-156">String</span><span class="sxs-lookup"><span data-stu-id="7032c-156">String</span></span>||
|<span data-ttu-id="7032c-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="7032c-157">postalCode</span></span>|<span data-ttu-id="7032c-158">String</span><span class="sxs-lookup"><span data-stu-id="7032c-158">String</span></span>||
|<span data-ttu-id="7032c-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="7032c-159">proxyAddresses</span></span>|<span data-ttu-id="7032c-160">String</span><span class="sxs-lookup"><span data-stu-id="7032c-160">String</span></span>||
|<span data-ttu-id="7032c-161">state</span><span class="sxs-lookup"><span data-stu-id="7032c-161">state</span></span>|<span data-ttu-id="7032c-162">Строка</span><span class="sxs-lookup"><span data-stu-id="7032c-162">String</span></span>||
|<span data-ttu-id="7032c-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="7032c-163">streetAddress</span></span>|<span data-ttu-id="7032c-164">String</span><span class="sxs-lookup"><span data-stu-id="7032c-164">String</span></span>||
|<span data-ttu-id="7032c-165">surname</span><span class="sxs-lookup"><span data-stu-id="7032c-165">surname</span></span>|<span data-ttu-id="7032c-166">String</span><span class="sxs-lookup"><span data-stu-id="7032c-166">String</span></span>||
|<span data-ttu-id="7032c-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="7032c-167">businessPhones</span></span>|<span data-ttu-id="7032c-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7032c-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="7032c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7032c-169">Response</span></span>

<span data-ttu-id="7032c-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7032c-170">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7032c-171">Пример</span><span class="sxs-lookup"><span data-stu-id="7032c-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7032c-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7032c-172">Request</span></span>
<span data-ttu-id="7032c-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7032c-173">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7032c-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="7032c-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7032c-175">C#</span><span class="sxs-lookup"><span data-stu-id="7032c-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7032c-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7032c-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7032c-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7032c-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7032c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="7032c-178">Response</span></span>
<span data-ttu-id="7032c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7032c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
