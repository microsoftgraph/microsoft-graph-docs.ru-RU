---
title: Обновление свойств educationSchool
description: Обновление свойств объекта school.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c7dd9cafe1238170599e802738d42bd287ebf47f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523647"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="729b9-103">Обновление свойств educationSchool</span><span class="sxs-lookup"><span data-stu-id="729b9-103">Update educationschool properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="729b9-104">Обновление свойств объекта school.</span><span class="sxs-lookup"><span data-stu-id="729b9-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="729b9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="729b9-105">Permissions</span></span>
<span data-ttu-id="729b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="729b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="729b9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="729b9-108">Permission type</span></span>      | <span data-ttu-id="729b9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="729b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="729b9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="729b9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="729b9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="729b9-111">Not supported.</span></span>  |
|<span data-ttu-id="729b9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="729b9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="729b9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="729b9-113">Not supported.</span></span>  |
|<span data-ttu-id="729b9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="729b9-114">Application</span></span> | <span data-ttu-id="729b9-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="729b9-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="729b9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="729b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="729b9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="729b9-117">Request headers</span></span>
| <span data-ttu-id="729b9-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="729b9-118">Header</span></span>       | <span data-ttu-id="729b9-119">Значение</span><span class="sxs-lookup"><span data-stu-id="729b9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="729b9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="729b9-120">Authorization</span></span>  | <span data-ttu-id="729b9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="729b9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="729b9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="729b9-123">Content-Type</span></span>  | <span data-ttu-id="729b9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="729b9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="729b9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="729b9-125">Request body</span></span>
<span data-ttu-id="729b9-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="729b9-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="729b9-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="729b9-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="729b9-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="729b9-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="729b9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="729b9-129">Property</span></span>     | <span data-ttu-id="729b9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="729b9-130">Type</span></span>   |<span data-ttu-id="729b9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="729b9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="729b9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="729b9-132">displayName</span></span>| <span data-ttu-id="729b9-133">String</span><span class="sxs-lookup"><span data-stu-id="729b9-133">String</span></span>| <span data-ttu-id="729b9-134">Отображаемое имя школы</span><span class="sxs-lookup"><span data-stu-id="729b9-134">Display name of the school</span></span>| 
|<span data-ttu-id="729b9-135">description</span><span class="sxs-lookup"><span data-stu-id="729b9-135">description</span></span>| <span data-ttu-id="729b9-136">Строка</span><span class="sxs-lookup"><span data-stu-id="729b9-136">String</span></span> | <span data-ttu-id="729b9-137">Описание школы</span><span class="sxs-lookup"><span data-stu-id="729b9-137">Description of the school</span></span>| 
|<span data-ttu-id="729b9-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="729b9-138">principalEmail</span></span>| <span data-ttu-id="729b9-139">String</span><span class="sxs-lookup"><span data-stu-id="729b9-139">String</span></span>| <span data-ttu-id="729b9-140">Адрес электронной почты директора</span><span class="sxs-lookup"><span data-stu-id="729b9-140">Email address of the principal</span></span>|
|<span data-ttu-id="729b9-141">principalName</span><span class="sxs-lookup"><span data-stu-id="729b9-141">principalName</span></span>| <span data-ttu-id="729b9-142">String</span><span class="sxs-lookup"><span data-stu-id="729b9-142">String</span></span> | <span data-ttu-id="729b9-143">Имя директора</span><span class="sxs-lookup"><span data-stu-id="729b9-143">Name of the principal</span></span>|
|<span data-ttu-id="729b9-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="729b9-144">externalPrincipalId</span></span>| <span data-ttu-id="729b9-145">String</span><span class="sxs-lookup"><span data-stu-id="729b9-145">String</span></span> | <span data-ttu-id="729b9-146">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="729b9-146">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="729b9-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="729b9-147">highestGrade</span></span>|<span data-ttu-id="729b9-148">String</span><span class="sxs-lookup"><span data-stu-id="729b9-148">String</span></span>| <span data-ttu-id="729b9-149">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="729b9-149">Highest grade taught.</span></span> |
|<span data-ttu-id="729b9-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="729b9-150">lowestGrade</span></span>|<span data-ttu-id="729b9-151">String</span><span class="sxs-lookup"><span data-stu-id="729b9-151">String</span></span>| <span data-ttu-id="729b9-152">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="729b9-152">Lowest grade taught.</span></span> |
|<span data-ttu-id="729b9-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="729b9-153">schoolNumber</span></span>|<span data-ttu-id="729b9-154">String</span><span class="sxs-lookup"><span data-stu-id="729b9-154">String</span></span>| <span data-ttu-id="729b9-155">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="729b9-155">School Number.</span></span>|
|<span data-ttu-id="729b9-156">externalId</span><span class="sxs-lookup"><span data-stu-id="729b9-156">externalId</span></span>|<span data-ttu-id="729b9-157">String</span><span class="sxs-lookup"><span data-stu-id="729b9-157">String</span></span>| <span data-ttu-id="729b9-158">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="729b9-158">Id of school in syncing system.</span></span> |
|<span data-ttu-id="729b9-159">phone</span><span class="sxs-lookup"><span data-stu-id="729b9-159">phone</span></span>|<span data-ttu-id="729b9-160">String</span><span class="sxs-lookup"><span data-stu-id="729b9-160">String</span></span>| <span data-ttu-id="729b9-161">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="729b9-161">Phone number of school.</span></span> |
|<span data-ttu-id="729b9-162">fax</span><span class="sxs-lookup"><span data-stu-id="729b9-162">fax</span></span>|<span data-ttu-id="729b9-163">String</span><span class="sxs-lookup"><span data-stu-id="729b9-163">String</span></span>| <span data-ttu-id="729b9-164">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="729b9-164">Fax number of school.</span></span> |
|<span data-ttu-id="729b9-165">address</span><span class="sxs-lookup"><span data-stu-id="729b9-165">address</span></span>|[<span data-ttu-id="729b9-166">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="729b9-166">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="729b9-167">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="729b9-167">Address of the School.</span></span>|
|<span data-ttu-id="729b9-168">createdBy</span><span class="sxs-lookup"><span data-stu-id="729b9-168">createdBy</span></span>|[<span data-ttu-id="729b9-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="729b9-169">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="729b9-170">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="729b9-170">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="729b9-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="729b9-171">Response</span></span>
<span data-ttu-id="729b9-172">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="729b9-172">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="729b9-173">Пример</span><span class="sxs-lookup"><span data-stu-id="729b9-173">Example</span></span>
##### <a name="request"></a><span data-ttu-id="729b9-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="729b9-174">Request</span></span>
<span data-ttu-id="729b9-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="729b9-175">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="729b9-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="729b9-176">Response</span></span>
<span data-ttu-id="729b9-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="729b9-177">The following is an example of the response.</span></span> 

><span data-ttu-id="729b9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="729b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/educationschool-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
