---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 32645e98fbb2e7da1aeec8d48eddb3c5da6822bb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054037"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="842ce-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="842ce-103">Update educationUser properties</span></span>

<span data-ttu-id="842ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="842ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="842ce-105">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="842ce-105">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="842ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="842ce-106">Permissions</span></span>
<span data-ttu-id="842ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="842ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="842ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="842ce-109">Permission type</span></span>      | <span data-ttu-id="842ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="842ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="842ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="842ce-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="842ce-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="842ce-112">Not supported.</span></span>  |
|<span data-ttu-id="842ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="842ce-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="842ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="842ce-114">Not supported.</span></span>  |
|<span data-ttu-id="842ce-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="842ce-115">Application</span></span> | <span data-ttu-id="842ce-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="842ce-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="842ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="842ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="842ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="842ce-118">Request headers</span></span>
| <span data-ttu-id="842ce-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="842ce-119">Header</span></span>       | <span data-ttu-id="842ce-120">Значение</span><span class="sxs-lookup"><span data-stu-id="842ce-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="842ce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="842ce-121">Authorization</span></span>  | <span data-ttu-id="842ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="842ce-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="842ce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="842ce-124">Content-Type</span></span>  | <span data-ttu-id="842ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="842ce-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="842ce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="842ce-126">Request body</span></span>
<span data-ttu-id="842ce-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="842ce-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="842ce-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="842ce-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="842ce-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="842ce-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="842ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="842ce-130">Property</span></span>     | <span data-ttu-id="842ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="842ce-131">Type</span></span>   |<span data-ttu-id="842ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="842ce-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="842ce-133">displayName</span><span class="sxs-lookup"><span data-stu-id="842ce-133">displayName</span></span>| <span data-ttu-id="842ce-134">String</span><span class="sxs-lookup"><span data-stu-id="842ce-134">String</span></span>| <span data-ttu-id="842ce-135">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="842ce-135">Display Name of User</span></span>|
|<span data-ttu-id="842ce-136">givenName;</span><span class="sxs-lookup"><span data-stu-id="842ce-136">givenName</span></span>| <span data-ttu-id="842ce-137">String</span><span class="sxs-lookup"><span data-stu-id="842ce-137">String</span></span> | <span data-ttu-id="842ce-138">Имя</span><span class="sxs-lookup"><span data-stu-id="842ce-138">First Name</span></span> |
|<span data-ttu-id="842ce-139">middleName</span><span class="sxs-lookup"><span data-stu-id="842ce-139">middleName</span></span>| <span data-ttu-id="842ce-140">String</span><span class="sxs-lookup"><span data-stu-id="842ce-140">String</span></span> | <span data-ttu-id="842ce-141">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="842ce-141">Middle Name of user</span></span>|
|<span data-ttu-id="842ce-142">surname</span><span class="sxs-lookup"><span data-stu-id="842ce-142">surname</span></span>| <span data-ttu-id="842ce-143">String</span><span class="sxs-lookup"><span data-stu-id="842ce-143">String</span></span> | <span data-ttu-id="842ce-144">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="842ce-144">Surname of user</span></span>|
|<span data-ttu-id="842ce-145">mail</span><span class="sxs-lookup"><span data-stu-id="842ce-145">mail</span></span>| <span data-ttu-id="842ce-146">String</span><span class="sxs-lookup"><span data-stu-id="842ce-146">String</span></span>| <span data-ttu-id="842ce-147">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="842ce-147">email address</span></span>|
|<span data-ttu-id="842ce-148">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="842ce-148">mobilePhone</span></span>| <span data-ttu-id="842ce-149">String</span><span class="sxs-lookup"><span data-stu-id="842ce-149">String</span></span> | <span data-ttu-id="842ce-150">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="842ce-150">Mobile number of user</span></span> |
|<span data-ttu-id="842ce-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="842ce-151">externalSource</span></span>|<span data-ttu-id="842ce-152">string</span><span class="sxs-lookup"><span data-stu-id="842ce-152">string</span></span>| <span data-ttu-id="842ce-153">Допустимые значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="842ce-153">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="842ce-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="842ce-154">externalSource</span></span>|<span data-ttu-id="842ce-155">string</span><span class="sxs-lookup"><span data-stu-id="842ce-155">string</span></span>| <span data-ttu-id="842ce-156">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="842ce-156">Where this user was created from.</span></span>  <span data-ttu-id="842ce-157">Допустимые значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="842ce-157">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="842ce-158">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="842ce-158">mailingAddress</span></span>|[<span data-ttu-id="842ce-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="842ce-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="842ce-160">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="842ce-160">Mail address of user.</span></span>|
|<span data-ttu-id="842ce-161">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="842ce-161">residenceAddress</span></span>|[<span data-ttu-id="842ce-162">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="842ce-162">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="842ce-163">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="842ce-163">Address where user lives.</span></span>|
|<span data-ttu-id="842ce-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="842ce-164">primaryRole</span></span>|<span data-ttu-id="842ce-165">string</span><span class="sxs-lookup"><span data-stu-id="842ce-165">string</span></span>| <span data-ttu-id="842ce-166">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="842ce-166">Default Role for a user.</span></span>  <span data-ttu-id="842ce-167">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="842ce-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="842ce-168">Допустимые значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="842ce-168">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="842ce-169">student</span><span class="sxs-lookup"><span data-stu-id="842ce-169">student</span></span>|[<span data-ttu-id="842ce-170">educationStudent</span><span class="sxs-lookup"><span data-stu-id="842ce-170">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="842ce-171">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="842ce-171">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="842ce-172">teacher</span><span class="sxs-lookup"><span data-stu-id="842ce-172">teacher</span></span>|[<span data-ttu-id="842ce-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="842ce-173">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="842ce-174">Если основной ролью является учитель, этот блок будет содержать определенные данные учителя.</span><span class="sxs-lookup"><span data-stu-id="842ce-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="842ce-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="842ce-175">Response</span></span>
<span data-ttu-id="842ce-176">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="842ce-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="842ce-177">Пример</span><span class="sxs-lookup"><span data-stu-id="842ce-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="842ce-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="842ce-178">Request</span></span>
<span data-ttu-id="842ce-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="842ce-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="842ce-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="842ce-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="842ce-181">C#</span><span class="sxs-lookup"><span data-stu-id="842ce-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="842ce-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="842ce-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="842ce-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="842ce-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="842ce-184">Java</span><span class="sxs-lookup"><span data-stu-id="842ce-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="842ce-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="842ce-185">Response</span></span>
<span data-ttu-id="842ce-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="842ce-186">Here is an example of the response.</span></span> <span data-ttu-id="842ce-187">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="842ce-187">Note: The response object shown here might be shortened for readability.</span></span>
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

