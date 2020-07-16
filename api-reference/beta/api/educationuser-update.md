---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 022b30eb68b29f4a77c34b0a8dc588d6f4bba071
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006770"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="b1827-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="b1827-103">Update educationUser properties</span></span>

<span data-ttu-id="b1827-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1827-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1827-105">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="b1827-105">Update the properties of an **educationuser** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1827-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1827-106">Permissions</span></span>

<span data-ttu-id="b1827-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1827-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1827-109">Permission type</span></span>                        | <span data-ttu-id="b1827-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1827-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b1827-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1827-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1827-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1827-112">Not supported.</span></span>                              |
| <span data-ttu-id="b1827-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1827-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1827-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1827-114">Not supported.</span></span>                              |
| <span data-ttu-id="b1827-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1827-115">Application</span></span>                            | <span data-ttu-id="b1827-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1827-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="b1827-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1827-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1827-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1827-118">Request headers</span></span>

| <span data-ttu-id="b1827-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1827-119">Header</span></span>        | <span data-ttu-id="b1827-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b1827-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="b1827-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1827-121">Authorization</span></span> | <span data-ttu-id="b1827-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1827-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b1827-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1827-124">Content-Type</span></span>  | <span data-ttu-id="b1827-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1827-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1827-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1827-127">Request body</span></span>

<span data-ttu-id="b1827-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b1827-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b1827-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b1827-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b1827-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b1827-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b1827-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1827-131">Property</span></span>         | <span data-ttu-id="b1827-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b1827-132">Type</span></span>               | <span data-ttu-id="b1827-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b1827-133">Description</span></span>                                                                                                                                     |
| :--------------- | :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b1827-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b1827-134">displayName</span></span>      | <span data-ttu-id="b1827-135">Строка</span><span class="sxs-lookup"><span data-stu-id="b1827-135">String</span></span>             | <span data-ttu-id="b1827-136">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b1827-136">Display Name of User</span></span>                                                                                                                            |
| <span data-ttu-id="b1827-137">givenName</span><span class="sxs-lookup"><span data-stu-id="b1827-137">givenName</span></span>        | <span data-ttu-id="b1827-138">String</span><span class="sxs-lookup"><span data-stu-id="b1827-138">String</span></span>             | <span data-ttu-id="b1827-139">Имя</span><span class="sxs-lookup"><span data-stu-id="b1827-139">First Name</span></span>                                                                                                                                      |
| <span data-ttu-id="b1827-140">middleName</span><span class="sxs-lookup"><span data-stu-id="b1827-140">middleName</span></span>       | <span data-ttu-id="b1827-141">String</span><span class="sxs-lookup"><span data-stu-id="b1827-141">String</span></span>             | <span data-ttu-id="b1827-142">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="b1827-142">Middle Name of user</span></span>                                                                                                                             |
| <span data-ttu-id="b1827-143">surname</span><span class="sxs-lookup"><span data-stu-id="b1827-143">surname</span></span>          | <span data-ttu-id="b1827-144">String</span><span class="sxs-lookup"><span data-stu-id="b1827-144">String</span></span>             | <span data-ttu-id="b1827-145">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="b1827-145">Surname of user</span></span>                                                                                                                                 |
| <span data-ttu-id="b1827-146">mail</span><span class="sxs-lookup"><span data-stu-id="b1827-146">mail</span></span>             | <span data-ttu-id="b1827-147">String</span><span class="sxs-lookup"><span data-stu-id="b1827-147">String</span></span>             | <span data-ttu-id="b1827-148">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="b1827-148">email address</span></span>                                                                                                                                   |
| <span data-ttu-id="b1827-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b1827-149">mobilePhone</span></span>      | <span data-ttu-id="b1827-150">String</span><span class="sxs-lookup"><span data-stu-id="b1827-150">String</span></span>             | <span data-ttu-id="b1827-151">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="b1827-151">Mobile number of user</span></span>                                                                                                                           |
| <span data-ttu-id="b1827-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="b1827-152">externalSource</span></span>   | <span data-ttu-id="b1827-153">string</span><span class="sxs-lookup"><span data-stu-id="b1827-153">string</span></span>             | <span data-ttu-id="b1827-154">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1827-154">Where this user was created from.</span></span> <span data-ttu-id="b1827-155">Возможные значения: `sis` , `manual` , или `lms` .</span><span class="sxs-lookup"><span data-stu-id="b1827-155">Possible values are: `sis`, `manual`, or `lms`.</span></span>                                                               |
| <span data-ttu-id="b1827-156">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="b1827-156">mailingAddress</span></span>   | <span data-ttu-id="b1827-157">[physicalAddress]</span><span class="sxs-lookup"><span data-stu-id="b1827-157">[physicalAddress]</span></span>  | <span data-ttu-id="b1827-158">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1827-158">Mail address of user.</span></span> <span data-ttu-id="b1827-159">Примечание: `type` и `postOfficeBox` не поддерживаются для `educationUser` ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b1827-159">Note: `type` and `postOfficeBox` are not supported for `educationUser` resources.</span></span>                                         |
| <span data-ttu-id="b1827-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="b1827-160">residenceAddress</span></span> | <span data-ttu-id="b1827-161">[physicalAddress]</span><span class="sxs-lookup"><span data-stu-id="b1827-161">[physicalAddress]</span></span>  | <span data-ttu-id="b1827-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1827-162">Address where user lives.</span></span> <span data-ttu-id="b1827-163">Примечание: `type` и `postOfficeBox` не поддерживаются для `educationUser` ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b1827-163">Note: `type` and `postOfficeBox` are not supported for `educationUser` resources.</span></span>                                     |
| <span data-ttu-id="b1827-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="b1827-164">primaryRole</span></span>      | <span data-ttu-id="b1827-165">string</span><span class="sxs-lookup"><span data-stu-id="b1827-165">string</span></span>             | <span data-ttu-id="b1827-166">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1827-166">Default Role for a user.</span></span> <span data-ttu-id="b1827-167">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="b1827-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="b1827-168">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="b1827-168">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span> |
| <span data-ttu-id="b1827-169">student</span><span class="sxs-lookup"><span data-stu-id="b1827-169">student</span></span>          | <span data-ttu-id="b1827-170">[educationStudent]</span><span class="sxs-lookup"><span data-stu-id="b1827-170">[educationStudent]</span></span> | <span data-ttu-id="b1827-171">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="b1827-171">If the primary role is student, this block will contain student specific data.</span></span>                                                                  |
| <span data-ttu-id="b1827-172">teacher</span><span class="sxs-lookup"><span data-stu-id="b1827-172">teacher</span></span>          | [<span data-ttu-id="b1827-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="b1827-173">educationTeacher</span></span>](../resources/educationteacher.md) | <span data-ttu-id="b1827-174">Если основная роль — преподаватель, этот блок будет содержать данные, характерные для преподавателя.</span><span class="sxs-lookup"><span data-stu-id="b1827-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>                                                                  |

## <a name="response"></a><span data-ttu-id="b1827-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1827-175">Response</span></span>

<span data-ttu-id="b1827-176">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1827-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1827-177">Пример</span><span class="sxs-lookup"><span data-stu-id="b1827-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1827-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1827-178">Request</span></span>

<span data-ttu-id="b1827-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1827-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1827-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1827-180">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="b1827-181">C#</span><span class="sxs-lookup"><span data-stu-id="b1827-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1827-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1827-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1827-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1827-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1827-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1827-184">Response</span></span>

<span data-ttu-id="b1827-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1827-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

[PhysicalAddress]: ../resources/physicaladdress.md
[physicaladdress]: ../resources/physicaladdress.md
[educationstudent]: ../resources/educationstudent.md
