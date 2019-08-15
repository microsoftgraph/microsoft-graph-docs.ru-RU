---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6b362533dbefb0e7ef9016babe7957ecbbb4990f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415829"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="e2f60-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="e2f60-103">Update educationUser properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2f60-104">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="e2f60-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2f60-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f60-105">Permissions</span></span>
<span data-ttu-id="e2f60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2f60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2f60-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f60-108">Permission type</span></span>      | <span data-ttu-id="e2f60-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2f60-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2f60-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2f60-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2f60-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f60-111">Not supported.</span></span>  |
|<span data-ttu-id="e2f60-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2f60-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e2f60-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f60-113">Not supported.</span></span>  |
|<span data-ttu-id="e2f60-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2f60-114">Application</span></span> | <span data-ttu-id="e2f60-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f60-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2f60-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2f60-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e2f60-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2f60-117">Request headers</span></span>
| <span data-ttu-id="e2f60-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2f60-118">Header</span></span>       | <span data-ttu-id="e2f60-119">Значение</span><span class="sxs-lookup"><span data-stu-id="e2f60-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2f60-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2f60-120">Authorization</span></span>  | <span data-ttu-id="e2f60-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2f60-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2f60-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2f60-123">Content-Type</span></span>  | <span data-ttu-id="e2f60-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e2f60-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2f60-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2f60-125">Request body</span></span>
<span data-ttu-id="e2f60-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e2f60-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e2f60-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e2f60-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e2f60-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e2f60-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e2f60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2f60-129">Property</span></span>     | <span data-ttu-id="e2f60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e2f60-130">Type</span></span>   |<span data-ttu-id="e2f60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e2f60-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2f60-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e2f60-132">displayName</span></span>| <span data-ttu-id="e2f60-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e2f60-133">String</span></span>| <span data-ttu-id="e2f60-134">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="e2f60-134">Display Name of User</span></span>|
|<span data-ttu-id="e2f60-135">givenName</span><span class="sxs-lookup"><span data-stu-id="e2f60-135">givenName</span></span>| <span data-ttu-id="e2f60-136">String</span><span class="sxs-lookup"><span data-stu-id="e2f60-136">String</span></span> | <span data-ttu-id="e2f60-137">Имя</span><span class="sxs-lookup"><span data-stu-id="e2f60-137">First Name</span></span> |
|<span data-ttu-id="e2f60-138">middleName</span><span class="sxs-lookup"><span data-stu-id="e2f60-138">middleName</span></span>| <span data-ttu-id="e2f60-139">String</span><span class="sxs-lookup"><span data-stu-id="e2f60-139">String</span></span> | <span data-ttu-id="e2f60-140">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="e2f60-140">Middle Name of user</span></span>|
|<span data-ttu-id="e2f60-141">surname</span><span class="sxs-lookup"><span data-stu-id="e2f60-141">surname</span></span>| <span data-ttu-id="e2f60-142">String</span><span class="sxs-lookup"><span data-stu-id="e2f60-142">String</span></span> | <span data-ttu-id="e2f60-143">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="e2f60-143">Surname of user</span></span>|
|<span data-ttu-id="e2f60-144">mail</span><span class="sxs-lookup"><span data-stu-id="e2f60-144">mail</span></span>| <span data-ttu-id="e2f60-145">String</span><span class="sxs-lookup"><span data-stu-id="e2f60-145">String</span></span>| <span data-ttu-id="e2f60-146">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="e2f60-146">email address</span></span>|
|<span data-ttu-id="e2f60-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e2f60-147">mobilePhone</span></span>| <span data-ttu-id="e2f60-148">String</span><span class="sxs-lookup"><span data-stu-id="e2f60-148">String</span></span> | <span data-ttu-id="e2f60-149">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="e2f60-149">Mobile number of user</span></span> |
|<span data-ttu-id="e2f60-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="e2f60-150">externalSource</span></span>|<span data-ttu-id="e2f60-151">string</span><span class="sxs-lookup"><span data-stu-id="e2f60-151">string</span></span>| <span data-ttu-id="e2f60-152">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="e2f60-152">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="e2f60-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="e2f60-153">externalSource</span></span>|<span data-ttu-id="e2f60-154">string</span><span class="sxs-lookup"><span data-stu-id="e2f60-154">string</span></span>| <span data-ttu-id="e2f60-155">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2f60-155">Where this user was created from.</span></span>  <span data-ttu-id="e2f60-156">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="e2f60-156">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="e2f60-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="e2f60-157">mailingAddress</span></span>|[<span data-ttu-id="e2f60-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e2f60-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="e2f60-159">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2f60-159">Mail address of user.</span></span>|
|<span data-ttu-id="e2f60-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="e2f60-160">residenceAddress</span></span>|[<span data-ttu-id="e2f60-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e2f60-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="e2f60-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2f60-162">Address where user lives.</span></span>|
|<span data-ttu-id="e2f60-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="e2f60-163">primaryRole</span></span>|<span data-ttu-id="e2f60-164">string</span><span class="sxs-lookup"><span data-stu-id="e2f60-164">string</span></span>| <span data-ttu-id="e2f60-165">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2f60-165">Default Role for a user.</span></span>  <span data-ttu-id="e2f60-166">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="e2f60-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="e2f60-167">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="e2f60-167">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="e2f60-168">student</span><span class="sxs-lookup"><span data-stu-id="e2f60-168">student</span></span>|[<span data-ttu-id="e2f60-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="e2f60-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="e2f60-170">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="e2f60-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="e2f60-171">teacher</span><span class="sxs-lookup"><span data-stu-id="e2f60-171">teacher</span></span>|[<span data-ttu-id="e2f60-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="e2f60-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="e2f60-173">Если основная роль — преподаватель, этот блок будет содержать данные, характерные для преподавателя.</span><span class="sxs-lookup"><span data-stu-id="e2f60-173">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="e2f60-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f60-174">Response</span></span>
<span data-ttu-id="e2f60-175">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2f60-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2f60-176">Пример</span><span class="sxs-lookup"><span data-stu-id="e2f60-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2f60-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2f60-177">Request</span></span>
<span data-ttu-id="e2f60-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2f60-178">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2f60-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2f60-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2f60-180">C#</span><span class="sxs-lookup"><span data-stu-id="e2f60-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2f60-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2f60-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2f60-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e2f60-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e2f60-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f60-183">Response</span></span>
<span data-ttu-id="e2f60-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2f60-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
