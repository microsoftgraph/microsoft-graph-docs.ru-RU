---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
ms.openlocfilehash: e5aa15075ac3e4f9386ac27d048ee339e7455b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026851"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="07764-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="07764-103">Update educationUser properties</span></span>

<span data-ttu-id="07764-104">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="07764-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="07764-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07764-105">Permissions</span></span>
<span data-ttu-id="07764-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07764-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07764-108">Permission type</span></span>      | <span data-ttu-id="07764-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07764-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07764-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07764-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="07764-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07764-111">Not supported.</span></span>  |
|<span data-ttu-id="07764-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07764-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="07764-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07764-113">Not supported.</span></span>  |
|<span data-ttu-id="07764-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07764-114">Application</span></span> | <span data-ttu-id="07764-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07764-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07764-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07764-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="07764-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07764-117">Request headers</span></span>
| <span data-ttu-id="07764-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07764-118">Header</span></span>       | <span data-ttu-id="07764-119">Значение</span><span class="sxs-lookup"><span data-stu-id="07764-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07764-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07764-120">Authorization</span></span>  | <span data-ttu-id="07764-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07764-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07764-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07764-123">Content-Type</span></span>  | <span data-ttu-id="07764-124">application/json</span><span class="sxs-lookup"><span data-stu-id="07764-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07764-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07764-125">Request body</span></span>
<span data-ttu-id="07764-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="07764-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="07764-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="07764-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07764-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="07764-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07764-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="07764-129">Property</span></span>     | <span data-ttu-id="07764-130">Тип</span><span class="sxs-lookup"><span data-stu-id="07764-130">Type</span></span>   |<span data-ttu-id="07764-131">Описание</span><span class="sxs-lookup"><span data-stu-id="07764-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07764-132">displayName</span><span class="sxs-lookup"><span data-stu-id="07764-132">displayName</span></span>| <span data-ttu-id="07764-133">String</span><span class="sxs-lookup"><span data-stu-id="07764-133">String</span></span>| <span data-ttu-id="07764-134">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="07764-134">Display Name of User</span></span>|
|<span data-ttu-id="07764-135">givenName</span><span class="sxs-lookup"><span data-stu-id="07764-135">givenName</span></span>| <span data-ttu-id="07764-136">String</span><span class="sxs-lookup"><span data-stu-id="07764-136">String</span></span> | <span data-ttu-id="07764-137">Имя</span><span class="sxs-lookup"><span data-stu-id="07764-137">First Name</span></span> |
|<span data-ttu-id="07764-138">middleName</span><span class="sxs-lookup"><span data-stu-id="07764-138">middleName</span></span>| <span data-ttu-id="07764-139">String</span><span class="sxs-lookup"><span data-stu-id="07764-139">String</span></span> | <span data-ttu-id="07764-140">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="07764-140">Middle Name of user</span></span>|
|<span data-ttu-id="07764-141">surname</span><span class="sxs-lookup"><span data-stu-id="07764-141">surname</span></span>| <span data-ttu-id="07764-142">String</span><span class="sxs-lookup"><span data-stu-id="07764-142">String</span></span> | <span data-ttu-id="07764-143">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="07764-143">Surname of user</span></span>|
|<span data-ttu-id="07764-144">mail</span><span class="sxs-lookup"><span data-stu-id="07764-144">mail</span></span>| <span data-ttu-id="07764-145">String</span><span class="sxs-lookup"><span data-stu-id="07764-145">String</span></span>| <span data-ttu-id="07764-146">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="07764-146">email address</span></span>|
|<span data-ttu-id="07764-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="07764-147">mobilePhone</span></span>| <span data-ttu-id="07764-148">String</span><span class="sxs-lookup"><span data-stu-id="07764-148">String</span></span> | <span data-ttu-id="07764-149">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="07764-149">Mobile number of user</span></span> |
|<span data-ttu-id="07764-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="07764-150">externalSource</span></span>|<span data-ttu-id="07764-151">string</span><span class="sxs-lookup"><span data-stu-id="07764-151">string</span></span>| <span data-ttu-id="07764-152">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="07764-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="07764-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="07764-153">externalSource</span></span>|<span data-ttu-id="07764-154">string</span><span class="sxs-lookup"><span data-stu-id="07764-154">string</span></span>| <span data-ttu-id="07764-155">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="07764-155">Where this user was created from.</span></span>  <span data-ttu-id="07764-156">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="07764-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="07764-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="07764-157">mailingAddress</span></span>|[<span data-ttu-id="07764-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="07764-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="07764-159">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="07764-159">Mail address of user.</span></span>|
|<span data-ttu-id="07764-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="07764-160">residenceAddress</span></span>|[<span data-ttu-id="07764-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="07764-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="07764-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="07764-162">Address where user lives.</span></span>|
|<span data-ttu-id="07764-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="07764-163">primaryRole</span></span>|<span data-ttu-id="07764-164">string</span><span class="sxs-lookup"><span data-stu-id="07764-164">string</span></span>| <span data-ttu-id="07764-165">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="07764-165">Default Role for a user.</span></span>  <span data-ttu-id="07764-166">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="07764-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="07764-167">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="07764-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="07764-168">student</span><span class="sxs-lookup"><span data-stu-id="07764-168">student</span></span>|[<span data-ttu-id="07764-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="07764-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="07764-170">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="07764-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="07764-171">teacher</span><span class="sxs-lookup"><span data-stu-id="07764-171">teacher</span></span>|[<span data-ttu-id="07764-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="07764-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="07764-173">Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.</span><span class="sxs-lookup"><span data-stu-id="07764-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="07764-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="07764-174">Response</span></span>
<span data-ttu-id="07764-175">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="07764-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07764-176">Пример</span><span class="sxs-lookup"><span data-stu-id="07764-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07764-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="07764-177">Request</span></span>
<span data-ttu-id="07764-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07764-178">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="07764-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="07764-179">Response</span></span>
<span data-ttu-id="07764-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="07764-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->