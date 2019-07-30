---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e38f555d9264ecf2280a2b09a97264ebee7bc96e
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932077"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="0efca-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="0efca-103">Update educationUser properties</span></span>

<span data-ttu-id="0efca-104">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="0efca-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0efca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0efca-105">Permissions</span></span>
<span data-ttu-id="0efca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0efca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0efca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0efca-108">Permission type</span></span>      | <span data-ttu-id="0efca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0efca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0efca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0efca-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0efca-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0efca-111">Not supported.</span></span>  |
|<span data-ttu-id="0efca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0efca-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0efca-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0efca-113">Not supported.</span></span>  |
|<span data-ttu-id="0efca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0efca-114">Application</span></span> | <span data-ttu-id="0efca-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0efca-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0efca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0efca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0efca-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0efca-117">Request headers</span></span>
| <span data-ttu-id="0efca-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0efca-118">Header</span></span>       | <span data-ttu-id="0efca-119">Значение</span><span class="sxs-lookup"><span data-stu-id="0efca-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0efca-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0efca-120">Authorization</span></span>  | <span data-ttu-id="0efca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0efca-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0efca-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0efca-123">Content-Type</span></span>  | <span data-ttu-id="0efca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0efca-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0efca-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0efca-125">Request body</span></span>
<span data-ttu-id="0efca-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0efca-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0efca-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0efca-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0efca-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0efca-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0efca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0efca-129">Property</span></span>     | <span data-ttu-id="0efca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0efca-130">Type</span></span>   |<span data-ttu-id="0efca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0efca-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0efca-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0efca-132">displayName</span></span>| <span data-ttu-id="0efca-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0efca-133">String</span></span>| <span data-ttu-id="0efca-134">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="0efca-134">Display Name of User</span></span>|
|<span data-ttu-id="0efca-135">givenName</span><span class="sxs-lookup"><span data-stu-id="0efca-135">givenName</span></span>| <span data-ttu-id="0efca-136">String</span><span class="sxs-lookup"><span data-stu-id="0efca-136">String</span></span> | <span data-ttu-id="0efca-137">Имя</span><span class="sxs-lookup"><span data-stu-id="0efca-137">First Name</span></span> |
|<span data-ttu-id="0efca-138">middleName</span><span class="sxs-lookup"><span data-stu-id="0efca-138">middleName</span></span>| <span data-ttu-id="0efca-139">String</span><span class="sxs-lookup"><span data-stu-id="0efca-139">String</span></span> | <span data-ttu-id="0efca-140">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="0efca-140">Middle Name of user</span></span>|
|<span data-ttu-id="0efca-141">surname</span><span class="sxs-lookup"><span data-stu-id="0efca-141">surname</span></span>| <span data-ttu-id="0efca-142">String</span><span class="sxs-lookup"><span data-stu-id="0efca-142">String</span></span> | <span data-ttu-id="0efca-143">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="0efca-143">Surname of user</span></span>|
|<span data-ttu-id="0efca-144">mail</span><span class="sxs-lookup"><span data-stu-id="0efca-144">mail</span></span>| <span data-ttu-id="0efca-145">String</span><span class="sxs-lookup"><span data-stu-id="0efca-145">String</span></span>| <span data-ttu-id="0efca-146">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="0efca-146">email address</span></span>|
|<span data-ttu-id="0efca-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0efca-147">mobilePhone</span></span>| <span data-ttu-id="0efca-148">String</span><span class="sxs-lookup"><span data-stu-id="0efca-148">String</span></span> | <span data-ttu-id="0efca-149">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="0efca-149">Mobile number of user</span></span> |
|<span data-ttu-id="0efca-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="0efca-150">externalSource</span></span>|<span data-ttu-id="0efca-151">string</span><span class="sxs-lookup"><span data-stu-id="0efca-151">string</span></span>| <span data-ttu-id="0efca-152">Допустимые значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="0efca-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="0efca-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="0efca-153">externalSource</span></span>|<span data-ttu-id="0efca-154">string</span><span class="sxs-lookup"><span data-stu-id="0efca-154">string</span></span>| <span data-ttu-id="0efca-155">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="0efca-155">Where this user was created from.</span></span>  <span data-ttu-id="0efca-156">Допустимые значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="0efca-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="0efca-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="0efca-157">mailingAddress</span></span>|[<span data-ttu-id="0efca-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0efca-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="0efca-159">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="0efca-159">Mail address of user.</span></span>|
|<span data-ttu-id="0efca-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="0efca-160">residenceAddress</span></span>|[<span data-ttu-id="0efca-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0efca-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="0efca-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="0efca-162">Address where user lives.</span></span>|
|<span data-ttu-id="0efca-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="0efca-163">primaryRole</span></span>|<span data-ttu-id="0efca-164">string</span><span class="sxs-lookup"><span data-stu-id="0efca-164">string</span></span>| <span data-ttu-id="0efca-165">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0efca-165">Default Role for a user.</span></span>  <span data-ttu-id="0efca-166">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="0efca-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="0efca-167">Допустимые значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="0efca-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="0efca-168">student</span><span class="sxs-lookup"><span data-stu-id="0efca-168">student</span></span>|[<span data-ttu-id="0efca-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="0efca-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="0efca-170">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="0efca-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="0efca-171">teacher</span><span class="sxs-lookup"><span data-stu-id="0efca-171">teacher</span></span>|[<span data-ttu-id="0efca-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="0efca-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="0efca-173">Если основная роль — преподаватель, этот блок будет содержать данные, характерные для преподавателя.</span><span class="sxs-lookup"><span data-stu-id="0efca-173">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="0efca-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="0efca-174">Response</span></span>
<span data-ttu-id="0efca-175">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0efca-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0efca-176">Пример</span><span class="sxs-lookup"><span data-stu-id="0efca-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0efca-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="0efca-177">Request</span></span>
<span data-ttu-id="0efca-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0efca-178">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0efca-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="0efca-179">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0efca-180">C#</span><span class="sxs-lookup"><span data-stu-id="0efca-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0efca-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="0efca-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0efca-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0efca-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0efca-183">Java</span><span class="sxs-lookup"><span data-stu-id="0efca-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0efca-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="0efca-184">Response</span></span>
<span data-ttu-id="0efca-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0efca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
