---
title: Обновление свойств educationSchool
description: Обновление свойств объекта school.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 23c7c476e2447fbde43a0e7521d4b3d626f80f5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892234"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="70918-103">Обновление свойств educationSchool</span><span class="sxs-lookup"><span data-stu-id="70918-103">Update educationschool properties</span></span>

> <span data-ttu-id="70918-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70918-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70918-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70918-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70918-106">Обновление свойств объекта school.</span><span class="sxs-lookup"><span data-stu-id="70918-106">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70918-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70918-107">Permissions</span></span>
<span data-ttu-id="70918-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70918-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70918-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70918-110">Permission type</span></span>      | <span data-ttu-id="70918-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70918-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70918-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70918-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="70918-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70918-113">Not supported.</span></span>  |
|<span data-ttu-id="70918-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70918-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="70918-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70918-115">Not supported.</span></span>  |
|<span data-ttu-id="70918-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70918-116">Application</span></span> | <span data-ttu-id="70918-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70918-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70918-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70918-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="70918-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70918-119">Request headers</span></span>
| <span data-ttu-id="70918-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70918-120">Header</span></span>       | <span data-ttu-id="70918-121">Значение</span><span class="sxs-lookup"><span data-stu-id="70918-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70918-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70918-122">Authorization</span></span>  | <span data-ttu-id="70918-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70918-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70918-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70918-125">Content-Type</span></span>  | <span data-ttu-id="70918-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70918-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70918-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70918-127">Request body</span></span>
<span data-ttu-id="70918-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="70918-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="70918-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="70918-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="70918-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="70918-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="70918-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="70918-131">Property</span></span>     | <span data-ttu-id="70918-132">Тип</span><span class="sxs-lookup"><span data-stu-id="70918-132">Type</span></span>   |<span data-ttu-id="70918-133">Описание</span><span class="sxs-lookup"><span data-stu-id="70918-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70918-134">displayName</span><span class="sxs-lookup"><span data-stu-id="70918-134">displayName</span></span>| <span data-ttu-id="70918-135">String</span><span class="sxs-lookup"><span data-stu-id="70918-135">String</span></span>| <span data-ttu-id="70918-136">Отображаемое имя школы</span><span class="sxs-lookup"><span data-stu-id="70918-136">Display name of the school</span></span>| 
|<span data-ttu-id="70918-137">описание</span><span class="sxs-lookup"><span data-stu-id="70918-137">description</span></span>| <span data-ttu-id="70918-138">String</span><span class="sxs-lookup"><span data-stu-id="70918-138">String</span></span> | <span data-ttu-id="70918-139">Описание школы</span><span class="sxs-lookup"><span data-stu-id="70918-139">Description of the school</span></span>| 
|<span data-ttu-id="70918-140">principalEmail</span><span class="sxs-lookup"><span data-stu-id="70918-140">principalEmail</span></span>| <span data-ttu-id="70918-141">String</span><span class="sxs-lookup"><span data-stu-id="70918-141">String</span></span>| <span data-ttu-id="70918-142">Адрес электронной почты директора</span><span class="sxs-lookup"><span data-stu-id="70918-142">Email address of the principal</span></span>|
|<span data-ttu-id="70918-143">principalName</span><span class="sxs-lookup"><span data-stu-id="70918-143">principalName</span></span>| <span data-ttu-id="70918-144">String</span><span class="sxs-lookup"><span data-stu-id="70918-144">String</span></span> | <span data-ttu-id="70918-145">Имя директора</span><span class="sxs-lookup"><span data-stu-id="70918-145">Name of the principal</span></span>|
|<span data-ttu-id="70918-146">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="70918-146">externalPrincipalId</span></span>| <span data-ttu-id="70918-147">String</span><span class="sxs-lookup"><span data-stu-id="70918-147">String</span></span> | <span data-ttu-id="70918-148">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="70918-148">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="70918-149">highestGrade</span><span class="sxs-lookup"><span data-stu-id="70918-149">highestGrade</span></span>|<span data-ttu-id="70918-150">String</span><span class="sxs-lookup"><span data-stu-id="70918-150">String</span></span>| <span data-ttu-id="70918-151">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="70918-151">Highest grade taught.</span></span> |
|<span data-ttu-id="70918-152">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="70918-152">lowestGrade</span></span>|<span data-ttu-id="70918-153">String</span><span class="sxs-lookup"><span data-stu-id="70918-153">String</span></span>| <span data-ttu-id="70918-154">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="70918-154">Lowest grade taught.</span></span> |
|<span data-ttu-id="70918-155">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="70918-155">schoolNumber</span></span>|<span data-ttu-id="70918-156">String</span><span class="sxs-lookup"><span data-stu-id="70918-156">String</span></span>| <span data-ttu-id="70918-157">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="70918-157">School Number.</span></span>|
|<span data-ttu-id="70918-158">externalId</span><span class="sxs-lookup"><span data-stu-id="70918-158">externalId</span></span>|<span data-ttu-id="70918-159">String</span><span class="sxs-lookup"><span data-stu-id="70918-159">String</span></span>| <span data-ttu-id="70918-160">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="70918-160">Id of school in syncing system.</span></span> |
|<span data-ttu-id="70918-161">phone</span><span class="sxs-lookup"><span data-stu-id="70918-161">phone</span></span>|<span data-ttu-id="70918-162">String</span><span class="sxs-lookup"><span data-stu-id="70918-162">String</span></span>| <span data-ttu-id="70918-163">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="70918-163">Phone number of school.</span></span> |
|<span data-ttu-id="70918-164">fax</span><span class="sxs-lookup"><span data-stu-id="70918-164">fax</span></span>|<span data-ttu-id="70918-165">String</span><span class="sxs-lookup"><span data-stu-id="70918-165">String</span></span>| <span data-ttu-id="70918-166">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="70918-166">Fax number of school.</span></span> |
|<span data-ttu-id="70918-167">address</span><span class="sxs-lookup"><span data-stu-id="70918-167">address</span></span>|[<span data-ttu-id="70918-168">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="70918-168">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="70918-169">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="70918-169">Address of the School.</span></span>|
|<span data-ttu-id="70918-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="70918-170">createdBy</span></span>|[<span data-ttu-id="70918-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="70918-171">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="70918-172">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="70918-172">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="70918-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="70918-173">Response</span></span>
<span data-ttu-id="70918-174">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="70918-174">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70918-175">Пример</span><span class="sxs-lookup"><span data-stu-id="70918-175">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70918-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="70918-176">Request</span></span>
<span data-ttu-id="70918-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70918-177">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="70918-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="70918-178">Response</span></span>
<span data-ttu-id="70918-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70918-179">The following is an example of the response.</span></span> 

><span data-ttu-id="70918-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70918-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
