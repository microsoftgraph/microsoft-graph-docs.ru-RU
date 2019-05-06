---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 959be23764b5348c0e9473aa00205620f321ebb4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596611"
---
# <a name="update-orgcontact"></a><span data-ttu-id="047c5-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="047c5-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="047c5-104">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="047c5-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="047c5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="047c5-105">Permissions</span></span>
<span data-ttu-id="047c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="047c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="047c5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="047c5-108">Permission type</span></span>      | <span data-ttu-id="047c5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="047c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="047c5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="047c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="047c5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="047c5-111">Not supported.</span></span>    |
|<span data-ttu-id="047c5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="047c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="047c5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="047c5-113">Not supported.</span></span>    |
|<span data-ttu-id="047c5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="047c5-114">Application</span></span> | <span data-ttu-id="047c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="047c5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="047c5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="047c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="047c5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="047c5-117">Request headers</span></span>
| <span data-ttu-id="047c5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="047c5-118">Name</span></span>       | <span data-ttu-id="047c5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="047c5-119">Type</span></span> | <span data-ttu-id="047c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="047c5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="047c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="047c5-121">Authorization</span></span>  | <span data-ttu-id="047c5-122">string</span><span class="sxs-lookup"><span data-stu-id="047c5-122">string</span></span>  | <span data-ttu-id="047c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="047c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="047c5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="047c5-125">Request body</span></span>
<span data-ttu-id="047c5-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="047c5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="047c5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="047c5-129">Property</span></span>     | <span data-ttu-id="047c5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="047c5-130">Type</span></span>   |<span data-ttu-id="047c5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="047c5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="047c5-132">city</span><span class="sxs-lookup"><span data-stu-id="047c5-132">city</span></span>|<span data-ttu-id="047c5-133">String</span><span class="sxs-lookup"><span data-stu-id="047c5-133">String</span></span>||
|<span data-ttu-id="047c5-134">country</span><span class="sxs-lookup"><span data-stu-id="047c5-134">country</span></span>|<span data-ttu-id="047c5-135">String</span><span class="sxs-lookup"><span data-stu-id="047c5-135">String</span></span>||
|<span data-ttu-id="047c5-136">department</span><span class="sxs-lookup"><span data-stu-id="047c5-136">department</span></span>|<span data-ttu-id="047c5-137">String</span><span class="sxs-lookup"><span data-stu-id="047c5-137">String</span></span>||
|<span data-ttu-id="047c5-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="047c5-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="047c5-139">Логический</span><span class="sxs-lookup"><span data-stu-id="047c5-139">Boolean</span></span>||
|<span data-ttu-id="047c5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="047c5-140">displayName</span></span>|<span data-ttu-id="047c5-141">Строка</span><span class="sxs-lookup"><span data-stu-id="047c5-141">String</span></span>||
|<span data-ttu-id="047c5-142">givenName</span><span class="sxs-lookup"><span data-stu-id="047c5-142">givenName</span></span>|<span data-ttu-id="047c5-143">String</span><span class="sxs-lookup"><span data-stu-id="047c5-143">String</span></span>||
|<span data-ttu-id="047c5-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="047c5-144">jobTitle</span></span>|<span data-ttu-id="047c5-145">String</span><span class="sxs-lookup"><span data-stu-id="047c5-145">String</span></span>||
|<span data-ttu-id="047c5-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="047c5-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="047c5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="047c5-147">DateTimeOffset</span></span>||
|<span data-ttu-id="047c5-148">mail</span><span class="sxs-lookup"><span data-stu-id="047c5-148">mail</span></span>|<span data-ttu-id="047c5-149">String</span><span class="sxs-lookup"><span data-stu-id="047c5-149">String</span></span>||
|<span data-ttu-id="047c5-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="047c5-150">mailNickname</span></span>|<span data-ttu-id="047c5-151">String</span><span class="sxs-lookup"><span data-stu-id="047c5-151">String</span></span>||
|<span data-ttu-id="047c5-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="047c5-152">mobilePhone</span></span>|<span data-ttu-id="047c5-153">String</span><span class="sxs-lookup"><span data-stu-id="047c5-153">String</span></span>||
|<span data-ttu-id="047c5-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="047c5-154">officeLocation</span></span>|<span data-ttu-id="047c5-155">String</span><span class="sxs-lookup"><span data-stu-id="047c5-155">String</span></span>||
|<span data-ttu-id="047c5-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="047c5-156">postalCode</span></span>|<span data-ttu-id="047c5-157">String</span><span class="sxs-lookup"><span data-stu-id="047c5-157">String</span></span>||
|<span data-ttu-id="047c5-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="047c5-158">proxyAddresses</span></span>|<span data-ttu-id="047c5-159">String</span><span class="sxs-lookup"><span data-stu-id="047c5-159">String</span></span>||
|<span data-ttu-id="047c5-160">state</span><span class="sxs-lookup"><span data-stu-id="047c5-160">state</span></span>|<span data-ttu-id="047c5-161">Строка</span><span class="sxs-lookup"><span data-stu-id="047c5-161">String</span></span>||
|<span data-ttu-id="047c5-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="047c5-162">streetAddress</span></span>|<span data-ttu-id="047c5-163">String</span><span class="sxs-lookup"><span data-stu-id="047c5-163">String</span></span>||
|<span data-ttu-id="047c5-164">surname</span><span class="sxs-lookup"><span data-stu-id="047c5-164">surname</span></span>|<span data-ttu-id="047c5-165">String</span><span class="sxs-lookup"><span data-stu-id="047c5-165">String</span></span>||
|<span data-ttu-id="047c5-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="047c5-166">businessPhones</span></span>|<span data-ttu-id="047c5-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="047c5-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="047c5-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="047c5-168">Response</span></span>

<span data-ttu-id="047c5-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="047c5-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="047c5-170">Пример</span><span class="sxs-lookup"><span data-stu-id="047c5-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="047c5-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="047c5-171">Request</span></span>
<span data-ttu-id="047c5-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="047c5-172">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="047c5-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="047c5-173">Response</span></span>
<span data-ttu-id="047c5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="047c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="047c5-177">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="047c5-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="047c5-178">Языках</span><span class="sxs-lookup"><span data-stu-id="047c5-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="047c5-179">Язык</span><span class="sxs-lookup"><span data-stu-id="047c5-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
