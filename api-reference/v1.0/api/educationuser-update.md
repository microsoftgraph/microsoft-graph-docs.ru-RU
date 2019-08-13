---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 35746d5945bc9b73491d67035c89139fd8d673e2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327635"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="356c8-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="356c8-103">Update educationUser properties</span></span>

<span data-ttu-id="356c8-104">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="356c8-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="356c8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="356c8-105">Permissions</span></span>
<span data-ttu-id="356c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="356c8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="356c8-108">Permission type</span></span>      | <span data-ttu-id="356c8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="356c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356c8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="356c8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="356c8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="356c8-111">Not supported.</span></span>  |
|<span data-ttu-id="356c8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="356c8-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="356c8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="356c8-113">Not supported.</span></span>  |
|<span data-ttu-id="356c8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="356c8-114">Application</span></span> | <span data-ttu-id="356c8-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356c8-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356c8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="356c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="356c8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="356c8-117">Request headers</span></span>
| <span data-ttu-id="356c8-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="356c8-118">Header</span></span>       | <span data-ttu-id="356c8-119">Значение</span><span class="sxs-lookup"><span data-stu-id="356c8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="356c8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="356c8-120">Authorization</span></span>  | <span data-ttu-id="356c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="356c8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="356c8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="356c8-123">Content-Type</span></span>  | <span data-ttu-id="356c8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="356c8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="356c8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="356c8-125">Request body</span></span>
<span data-ttu-id="356c8-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="356c8-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="356c8-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="356c8-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="356c8-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="356c8-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="356c8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="356c8-129">Property</span></span>     | <span data-ttu-id="356c8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="356c8-130">Type</span></span>   |<span data-ttu-id="356c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="356c8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="356c8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="356c8-132">displayName</span></span>| <span data-ttu-id="356c8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="356c8-133">String</span></span>| <span data-ttu-id="356c8-134">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="356c8-134">Display Name of User</span></span>|
|<span data-ttu-id="356c8-135">givenName</span><span class="sxs-lookup"><span data-stu-id="356c8-135">givenName</span></span>| <span data-ttu-id="356c8-136">String</span><span class="sxs-lookup"><span data-stu-id="356c8-136">String</span></span> | <span data-ttu-id="356c8-137">Имя</span><span class="sxs-lookup"><span data-stu-id="356c8-137">First Name</span></span> |
|<span data-ttu-id="356c8-138">middleName</span><span class="sxs-lookup"><span data-stu-id="356c8-138">middleName</span></span>| <span data-ttu-id="356c8-139">String</span><span class="sxs-lookup"><span data-stu-id="356c8-139">String</span></span> | <span data-ttu-id="356c8-140">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="356c8-140">Middle Name of user</span></span>|
|<span data-ttu-id="356c8-141">surname</span><span class="sxs-lookup"><span data-stu-id="356c8-141">surname</span></span>| <span data-ttu-id="356c8-142">String</span><span class="sxs-lookup"><span data-stu-id="356c8-142">String</span></span> | <span data-ttu-id="356c8-143">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="356c8-143">Surname of user</span></span>|
|<span data-ttu-id="356c8-144">mail</span><span class="sxs-lookup"><span data-stu-id="356c8-144">mail</span></span>| <span data-ttu-id="356c8-145">String</span><span class="sxs-lookup"><span data-stu-id="356c8-145">String</span></span>| <span data-ttu-id="356c8-146">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="356c8-146">email address</span></span>|
|<span data-ttu-id="356c8-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="356c8-147">mobilePhone</span></span>| <span data-ttu-id="356c8-148">String</span><span class="sxs-lookup"><span data-stu-id="356c8-148">String</span></span> | <span data-ttu-id="356c8-149">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="356c8-149">Mobile number of user</span></span> |
|<span data-ttu-id="356c8-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="356c8-150">externalSource</span></span>|<span data-ttu-id="356c8-151">string</span><span class="sxs-lookup"><span data-stu-id="356c8-151">string</span></span>| <span data-ttu-id="356c8-152">Допустимые значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="356c8-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="356c8-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="356c8-153">externalSource</span></span>|<span data-ttu-id="356c8-154">string</span><span class="sxs-lookup"><span data-stu-id="356c8-154">string</span></span>| <span data-ttu-id="356c8-155">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="356c8-155">Where this user was created from.</span></span>  <span data-ttu-id="356c8-156">Допустимые значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="356c8-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="356c8-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="356c8-157">mailingAddress</span></span>|[<span data-ttu-id="356c8-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="356c8-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="356c8-159">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="356c8-159">Mail address of user.</span></span>|
|<span data-ttu-id="356c8-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="356c8-160">residenceAddress</span></span>|[<span data-ttu-id="356c8-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="356c8-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="356c8-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="356c8-162">Address where user lives.</span></span>|
|<span data-ttu-id="356c8-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="356c8-163">primaryRole</span></span>|<span data-ttu-id="356c8-164">string</span><span class="sxs-lookup"><span data-stu-id="356c8-164">string</span></span>| <span data-ttu-id="356c8-165">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="356c8-165">Default Role for a user.</span></span>  <span data-ttu-id="356c8-166">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="356c8-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="356c8-167">Допустимые значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="356c8-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="356c8-168">student</span><span class="sxs-lookup"><span data-stu-id="356c8-168">student</span></span>|[<span data-ttu-id="356c8-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="356c8-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="356c8-170">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="356c8-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="356c8-171">teacher</span><span class="sxs-lookup"><span data-stu-id="356c8-171">teacher</span></span>|[<span data-ttu-id="356c8-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="356c8-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="356c8-173">Если основная роль — преподаватель, этот блок будет содержать данные, характерные для преподавателя.</span><span class="sxs-lookup"><span data-stu-id="356c8-173">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="356c8-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="356c8-174">Response</span></span>
<span data-ttu-id="356c8-175">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="356c8-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="356c8-176">Пример</span><span class="sxs-lookup"><span data-stu-id="356c8-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="356c8-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="356c8-177">Request</span></span>
<span data-ttu-id="356c8-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="356c8-178">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="356c8-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="356c8-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="356c8-180">C#</span><span class="sxs-lookup"><span data-stu-id="356c8-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="356c8-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="356c8-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="356c8-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="356c8-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="356c8-183">Java</span><span class="sxs-lookup"><span data-stu-id="356c8-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="356c8-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="356c8-184">Response</span></span>
<span data-ttu-id="356c8-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="356c8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
