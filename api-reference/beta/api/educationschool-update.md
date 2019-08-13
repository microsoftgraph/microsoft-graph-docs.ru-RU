---
title: Обновление свойств educationSchool
description: Обновление свойств объекта school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 99bd6e38c5f91d06586539a9cdb2c9e2243055e0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323838"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="d7d64-103">Обновление свойств educationSchool</span><span class="sxs-lookup"><span data-stu-id="d7d64-103">Update educationschool properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d64-104">Обновление свойств объекта school.</span><span class="sxs-lookup"><span data-stu-id="d7d64-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7d64-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d64-105">Permissions</span></span>
<span data-ttu-id="d7d64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7d64-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d64-108">Permission type</span></span>      | <span data-ttu-id="d7d64-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7d64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7d64-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7d64-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d7d64-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d64-111">Not supported.</span></span>  |
|<span data-ttu-id="d7d64-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7d64-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d7d64-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d64-113">Not supported.</span></span>  |
|<span data-ttu-id="d7d64-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7d64-114">Application</span></span> | <span data-ttu-id="d7d64-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d64-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7d64-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7d64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d7d64-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7d64-117">Request headers</span></span>
| <span data-ttu-id="d7d64-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7d64-118">Header</span></span>       | <span data-ttu-id="d7d64-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d7d64-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7d64-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7d64-120">Authorization</span></span>  | <span data-ttu-id="d7d64-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7d64-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7d64-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7d64-123">Content-Type</span></span>  | <span data-ttu-id="d7d64-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d7d64-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7d64-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7d64-125">Request body</span></span>
<span data-ttu-id="d7d64-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d7d64-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d7d64-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d7d64-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d7d64-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d7d64-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7d64-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d64-129">Property</span></span>     | <span data-ttu-id="d7d64-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d64-130">Type</span></span>   |<span data-ttu-id="d7d64-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d64-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7d64-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d7d64-132">displayName</span></span>| <span data-ttu-id="d7d64-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d64-133">String</span></span>| <span data-ttu-id="d7d64-134">Отображаемое имя школы</span><span class="sxs-lookup"><span data-stu-id="d7d64-134">Display name of the school</span></span>| 
|<span data-ttu-id="d7d64-135">description</span><span class="sxs-lookup"><span data-stu-id="d7d64-135">description</span></span>| <span data-ttu-id="d7d64-136">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-136">String</span></span> | <span data-ttu-id="d7d64-137">Описание школы</span><span class="sxs-lookup"><span data-stu-id="d7d64-137">Description of the school</span></span>| 
|<span data-ttu-id="d7d64-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="d7d64-138">principalEmail</span></span>| <span data-ttu-id="d7d64-139">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-139">String</span></span>| <span data-ttu-id="d7d64-140">Адрес электронной почты директора</span><span class="sxs-lookup"><span data-stu-id="d7d64-140">Email address of the principal</span></span>|
|<span data-ttu-id="d7d64-141">principalName</span><span class="sxs-lookup"><span data-stu-id="d7d64-141">principalName</span></span>| <span data-ttu-id="d7d64-142">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-142">String</span></span> | <span data-ttu-id="d7d64-143">Имя директора</span><span class="sxs-lookup"><span data-stu-id="d7d64-143">Name of the principal</span></span>|
|<span data-ttu-id="d7d64-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="d7d64-144">externalPrincipalId</span></span>| <span data-ttu-id="d7d64-145">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-145">String</span></span> | <span data-ttu-id="d7d64-146">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d7d64-146">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="d7d64-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="d7d64-147">highestGrade</span></span>|<span data-ttu-id="d7d64-148">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-148">String</span></span>| <span data-ttu-id="d7d64-149">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="d7d64-149">Highest grade taught.</span></span> |
|<span data-ttu-id="d7d64-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="d7d64-150">lowestGrade</span></span>|<span data-ttu-id="d7d64-151">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-151">String</span></span>| <span data-ttu-id="d7d64-152">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="d7d64-152">Lowest grade taught.</span></span> |
|<span data-ttu-id="d7d64-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="d7d64-153">schoolNumber</span></span>|<span data-ttu-id="d7d64-154">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-154">String</span></span>| <span data-ttu-id="d7d64-155">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="d7d64-155">School Number.</span></span>|
|<span data-ttu-id="d7d64-156">externalId</span><span class="sxs-lookup"><span data-stu-id="d7d64-156">externalId</span></span>|<span data-ttu-id="d7d64-157">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-157">String</span></span>| <span data-ttu-id="d7d64-158">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d7d64-158">Id of school in syncing system.</span></span> |
|<span data-ttu-id="d7d64-159">phone</span><span class="sxs-lookup"><span data-stu-id="d7d64-159">phone</span></span>|<span data-ttu-id="d7d64-160">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-160">String</span></span>| <span data-ttu-id="d7d64-161">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="d7d64-161">Phone number of school.</span></span> |
|<span data-ttu-id="d7d64-162">fax</span><span class="sxs-lookup"><span data-stu-id="d7d64-162">fax</span></span>|<span data-ttu-id="d7d64-163">String</span><span class="sxs-lookup"><span data-stu-id="d7d64-163">String</span></span>| <span data-ttu-id="d7d64-164">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="d7d64-164">Fax number of school.</span></span> |
|<span data-ttu-id="d7d64-165">address</span><span class="sxs-lookup"><span data-stu-id="d7d64-165">address</span></span>|[<span data-ttu-id="d7d64-166">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d7d64-166">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="d7d64-167">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="d7d64-167">Address of the School.</span></span>|
|<span data-ttu-id="d7d64-168">createdBy</span><span class="sxs-lookup"><span data-stu-id="d7d64-168">createdBy</span></span>|[<span data-ttu-id="d7d64-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="d7d64-169">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="d7d64-170">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="d7d64-170">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="d7d64-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d64-171">Response</span></span>
<span data-ttu-id="d7d64-172">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7d64-172">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7d64-173">Пример</span><span class="sxs-lookup"><span data-stu-id="d7d64-173">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7d64-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7d64-174">Request</span></span>
<span data-ttu-id="d7d64-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7d64-175">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7d64-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7d64-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7d64-177">C#</span><span class="sxs-lookup"><span data-stu-id="d7d64-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7d64-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7d64-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7d64-179">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d7d64-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d7d64-180">Java</span><span class="sxs-lookup"><span data-stu-id="d7d64-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7d64-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d64-181">Response</span></span>
<span data-ttu-id="d7d64-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7d64-182">The following is an example of the response.</span></span> 

><span data-ttu-id="d7d64-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7d64-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
