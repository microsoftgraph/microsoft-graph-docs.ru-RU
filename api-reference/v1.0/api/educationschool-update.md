---
title: Обновление educationSchool
description: Обновление свойств объекта educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e6c53b2b9b5934559a352378ee5316618ae69abe
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231873"
---
# <a name="update-educationschool"></a><span data-ttu-id="95cf1-103">Обновление educationSchool</span><span class="sxs-lookup"><span data-stu-id="95cf1-103">Update educationSchool</span></span>

<span data-ttu-id="95cf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95cf1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95cf1-105">Обновление свойств объекта [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="95cf1-105">Update the properties of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95cf1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95cf1-106">Permissions</span></span>

<span data-ttu-id="95cf1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95cf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95cf1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95cf1-109">Permission type</span></span>                        | <span data-ttu-id="95cf1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95cf1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="95cf1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95cf1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95cf1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95cf1-112">Not supported.</span></span>                              |
| <span data-ttu-id="95cf1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95cf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95cf1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95cf1-114">Not supported.</span></span>                              |
| <span data-ttu-id="95cf1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="95cf1-115">Application</span></span>                            | <span data-ttu-id="95cf1-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95cf1-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="95cf1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95cf1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="95cf1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95cf1-118">Request headers</span></span>

| <span data-ttu-id="95cf1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95cf1-119">Header</span></span>        | <span data-ttu-id="95cf1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="95cf1-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="95cf1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95cf1-121">Authorization</span></span> | <span data-ttu-id="95cf1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95cf1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="95cf1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95cf1-124">Content-Type</span></span>  | <span data-ttu-id="95cf1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95cf1-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="95cf1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95cf1-126">Request body</span></span>

<span data-ttu-id="95cf1-127">В теле запроса поставляем представление JSON объекта [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="95cf1-127">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="95cf1-128">В следующей таблице показаны свойства, необходимые при обновлении [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="95cf1-128">The following table shows the properties that are required when you update the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="95cf1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95cf1-129">Property</span></span>             | <span data-ttu-id="95cf1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95cf1-130">Type</span></span>                                               | <span data-ttu-id="95cf1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95cf1-131">Description</span></span>                                                                                                                                                           |
| :------------------- | :------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="95cf1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="95cf1-132">displayName</span></span>          | <span data-ttu-id="95cf1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="95cf1-133">String</span></span>                                             | <span data-ttu-id="95cf1-134">Отображаемое имя учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="95cf1-134">Display name of the school.</span></span> <span data-ttu-id="95cf1-135">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="95cf1-135">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="95cf1-136">description</span><span class="sxs-lookup"><span data-stu-id="95cf1-136">description</span></span>          | <span data-ttu-id="95cf1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="95cf1-137">String</span></span>                                             | <span data-ttu-id="95cf1-138">Описание учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="95cf1-138">Description of the school.</span></span> <span data-ttu-id="95cf1-139">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="95cf1-139">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                             |
| <span data-ttu-id="95cf1-140">externalSource</span><span class="sxs-lookup"><span data-stu-id="95cf1-140">externalSource</span></span>       | <span data-ttu-id="95cf1-141">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="95cf1-141">educationExternalSource</span></span>                            | <span data-ttu-id="95cf1-142">Источник, из которых была создана эта организация.</span><span class="sxs-lookup"><span data-stu-id="95cf1-142">Source where this organization was created from.</span></span> <span data-ttu-id="95cf1-143">Унаследованный от [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="95cf1-143">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="95cf1-144">Возможные значения: `sis`, `manual`.</span><span class="sxs-lookup"><span data-stu-id="95cf1-144">Possible values are: `sis`, `manual`.</span></span> |
| <span data-ttu-id="95cf1-145">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="95cf1-145">externalSourceDetail</span></span> | <span data-ttu-id="95cf1-146">Строка</span><span class="sxs-lookup"><span data-stu-id="95cf1-146">String</span></span>                                             | <span data-ttu-id="95cf1-147">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="95cf1-147">The name of the external source this resources was generated from.</span></span>                                                                                                    |
| <span data-ttu-id="95cf1-148">principalEmail</span><span class="sxs-lookup"><span data-stu-id="95cf1-148">principalEmail</span></span>       | <span data-ttu-id="95cf1-149">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-149">String</span></span>                                             | <span data-ttu-id="95cf1-150">Адрес электронной почты директора.</span><span class="sxs-lookup"><span data-stu-id="95cf1-150">Email address of the principal.</span></span>                                                                                                                                       |
| <span data-ttu-id="95cf1-151">principalName</span><span class="sxs-lookup"><span data-stu-id="95cf1-151">principalName</span></span>        | <span data-ttu-id="95cf1-152">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-152">String</span></span>                                             | <span data-ttu-id="95cf1-153">Имя директора.</span><span class="sxs-lookup"><span data-stu-id="95cf1-153">Name of the principal.</span></span>                                                                                                                                                |
| <span data-ttu-id="95cf1-154">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="95cf1-154">externalPrincipalId</span></span>  | <span data-ttu-id="95cf1-155">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-155">String</span></span>                                             | <span data-ttu-id="95cf1-156">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="95cf1-156">ID of principal in syncing system.</span></span>                                                                                                                                    |
| <span data-ttu-id="95cf1-157">highestGrade</span><span class="sxs-lookup"><span data-stu-id="95cf1-157">highestGrade</span></span>         | <span data-ttu-id="95cf1-158">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-158">String</span></span>                                             | <span data-ttu-id="95cf1-159">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="95cf1-159">Highest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="95cf1-160">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="95cf1-160">lowestGrade</span></span>          | <span data-ttu-id="95cf1-161">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-161">String</span></span>                                             | <span data-ttu-id="95cf1-162">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="95cf1-162">Lowest grade taught.</span></span>                                                                                                                                                  |
| <span data-ttu-id="95cf1-163">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="95cf1-163">schoolNumber</span></span>         | <span data-ttu-id="95cf1-164">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-164">String</span></span>                                             | <span data-ttu-id="95cf1-165">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="95cf1-165">School Number.</span></span>                                                                                                                                                        |
| <span data-ttu-id="95cf1-166">externalId</span><span class="sxs-lookup"><span data-stu-id="95cf1-166">externalId</span></span>           | <span data-ttu-id="95cf1-167">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-167">String</span></span>                                             | <span data-ttu-id="95cf1-168">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="95cf1-168">ID of school in syncing system.</span></span>                                                                                                                                       |
| <span data-ttu-id="95cf1-169">phone</span><span class="sxs-lookup"><span data-stu-id="95cf1-169">phone</span></span>                | <span data-ttu-id="95cf1-170">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-170">String</span></span>                                             | <span data-ttu-id="95cf1-171">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="95cf1-171">Phone number of school.</span></span>                                                                                                                                               |
| <span data-ttu-id="95cf1-172">fax</span><span class="sxs-lookup"><span data-stu-id="95cf1-172">fax</span></span>                  | <span data-ttu-id="95cf1-173">String</span><span class="sxs-lookup"><span data-stu-id="95cf1-173">String</span></span>                                             | <span data-ttu-id="95cf1-174">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="95cf1-174">Fax number of school.</span></span>                                                                                                                                                 |
| <span data-ttu-id="95cf1-175">createdBy</span><span class="sxs-lookup"><span data-stu-id="95cf1-175">createdBy</span></span>            | [<span data-ttu-id="95cf1-176">identitySet</span><span class="sxs-lookup"><span data-stu-id="95cf1-176">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="95cf1-177">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="95cf1-177">Entity who created the school.</span></span>                                                                                                                                        |
| <span data-ttu-id="95cf1-178">address</span><span class="sxs-lookup"><span data-stu-id="95cf1-178">address</span></span>              | [<span data-ttu-id="95cf1-179">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="95cf1-179">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="95cf1-180">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="95cf1-180">Address of the school.</span></span>                                                                                                                                                |

## <a name="response"></a><span data-ttu-id="95cf1-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="95cf1-181">Response</span></span>

<span data-ttu-id="95cf1-182">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95cf1-182">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95cf1-183">Пример</span><span class="sxs-lookup"><span data-stu-id="95cf1-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95cf1-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="95cf1-184">Request</span></span>

<span data-ttu-id="95cf1-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95cf1-185">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95cf1-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="95cf1-186">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```

# <a name="c"></a>[<span data-ttu-id="95cf1-187">C#</span><span class="sxs-lookup"><span data-stu-id="95cf1-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95cf1-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95cf1-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95cf1-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95cf1-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95cf1-190">Java</span><span class="sxs-lookup"><span data-stu-id="95cf1-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="95cf1-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="95cf1-191">Response</span></span>

<span data-ttu-id="95cf1-192">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="95cf1-192">The following is an example of the response.</span></span>

><span data-ttu-id="95cf1-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95cf1-193">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
