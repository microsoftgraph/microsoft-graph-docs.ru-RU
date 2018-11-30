---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
ms.openlocfilehash: bd8d8f95cf1c8475a5c52946d0cf0d1eaa5240ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076596"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="eb940-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="eb940-103">Update educationUser properties</span></span>

> <span data-ttu-id="eb940-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb940-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb940-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb940-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb940-106">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="eb940-106">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb940-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb940-107">Permissions</span></span>
<span data-ttu-id="eb940-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb940-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb940-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb940-110">Permission type</span></span>      | <span data-ttu-id="eb940-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb940-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb940-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb940-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="eb940-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb940-113">Not supported.</span></span>  |
|<span data-ttu-id="eb940-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb940-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="eb940-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb940-115">Not supported.</span></span>  |
|<span data-ttu-id="eb940-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb940-116">Application</span></span> | <span data-ttu-id="eb940-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb940-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb940-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb940-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eb940-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb940-119">Request headers</span></span>
| <span data-ttu-id="eb940-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb940-120">Header</span></span>       | <span data-ttu-id="eb940-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eb940-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb940-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb940-122">Authorization</span></span>  | <span data-ttu-id="eb940-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb940-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb940-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb940-125">Content-Type</span></span>  | <span data-ttu-id="eb940-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb940-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb940-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb940-127">Request body</span></span>
<span data-ttu-id="eb940-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="eb940-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eb940-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="eb940-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eb940-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="eb940-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eb940-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb940-131">Property</span></span>     | <span data-ttu-id="eb940-132">Тип</span><span class="sxs-lookup"><span data-stu-id="eb940-132">Type</span></span>   |<span data-ttu-id="eb940-133">Описание</span><span class="sxs-lookup"><span data-stu-id="eb940-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb940-134">displayName</span><span class="sxs-lookup"><span data-stu-id="eb940-134">displayName</span></span>| <span data-ttu-id="eb940-135">String</span><span class="sxs-lookup"><span data-stu-id="eb940-135">String</span></span>| <span data-ttu-id="eb940-136">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="eb940-136">Display Name of User</span></span>|
|<span data-ttu-id="eb940-137">givenName</span><span class="sxs-lookup"><span data-stu-id="eb940-137">givenName</span></span>| <span data-ttu-id="eb940-138">String</span><span class="sxs-lookup"><span data-stu-id="eb940-138">String</span></span> | <span data-ttu-id="eb940-139">Имя</span><span class="sxs-lookup"><span data-stu-id="eb940-139">First Name</span></span> |
|<span data-ttu-id="eb940-140">middleName</span><span class="sxs-lookup"><span data-stu-id="eb940-140">middleName</span></span>| <span data-ttu-id="eb940-141">String</span><span class="sxs-lookup"><span data-stu-id="eb940-141">String</span></span> | <span data-ttu-id="eb940-142">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="eb940-142">Middle Name of user</span></span>|
|<span data-ttu-id="eb940-143">surname</span><span class="sxs-lookup"><span data-stu-id="eb940-143">surname</span></span>| <span data-ttu-id="eb940-144">String</span><span class="sxs-lookup"><span data-stu-id="eb940-144">String</span></span> | <span data-ttu-id="eb940-145">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="eb940-145">Surname of user</span></span>|
|<span data-ttu-id="eb940-146">mail</span><span class="sxs-lookup"><span data-stu-id="eb940-146">mail</span></span>| <span data-ttu-id="eb940-147">String</span><span class="sxs-lookup"><span data-stu-id="eb940-147">String</span></span>| <span data-ttu-id="eb940-148">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="eb940-148">email address</span></span>|
|<span data-ttu-id="eb940-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="eb940-149">mobilePhone</span></span>| <span data-ttu-id="eb940-150">String</span><span class="sxs-lookup"><span data-stu-id="eb940-150">String</span></span> | <span data-ttu-id="eb940-151">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="eb940-151">Mobile number of user</span></span> |
|<span data-ttu-id="eb940-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="eb940-152">externalSource</span></span>|<span data-ttu-id="eb940-153">string</span><span class="sxs-lookup"><span data-stu-id="eb940-153">string</span></span>| <span data-ttu-id="eb940-154">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="eb940-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="eb940-155">externalSource</span><span class="sxs-lookup"><span data-stu-id="eb940-155">externalSource</span></span>|<span data-ttu-id="eb940-156">string</span><span class="sxs-lookup"><span data-stu-id="eb940-156">string</span></span>| <span data-ttu-id="eb940-157">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb940-157">Where this user was created from.</span></span>  <span data-ttu-id="eb940-158">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="eb940-158">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="eb940-159">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="eb940-159">mailingAddress</span></span>|[<span data-ttu-id="eb940-160">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="eb940-160">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="eb940-161">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb940-161">Mail address of user.</span></span>|
|<span data-ttu-id="eb940-162">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="eb940-162">residenceAddress</span></span>|[<span data-ttu-id="eb940-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="eb940-163">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="eb940-164">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb940-164">Address where user lives.</span></span>|
|<span data-ttu-id="eb940-165">primaryRole</span><span class="sxs-lookup"><span data-stu-id="eb940-165">primaryRole</span></span>|<span data-ttu-id="eb940-166">string</span><span class="sxs-lookup"><span data-stu-id="eb940-166">string</span></span>| <span data-ttu-id="eb940-167">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb940-167">Default Role for a user.</span></span>  <span data-ttu-id="eb940-168">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="eb940-168">The user's role might be different in an individual class.</span></span> <span data-ttu-id="eb940-169">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="eb940-169">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="eb940-170">student</span><span class="sxs-lookup"><span data-stu-id="eb940-170">student</span></span>|[<span data-ttu-id="eb940-171">educationStudent</span><span class="sxs-lookup"><span data-stu-id="eb940-171">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="eb940-172">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="eb940-172">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="eb940-173">teacher</span><span class="sxs-lookup"><span data-stu-id="eb940-173">teacher</span></span>|[<span data-ttu-id="eb940-174">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="eb940-174">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="eb940-175">Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.</span><span class="sxs-lookup"><span data-stu-id="eb940-175">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="eb940-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb940-176">Response</span></span>
<span data-ttu-id="eb940-177">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb940-177">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb940-178">Пример</span><span class="sxs-lookup"><span data-stu-id="eb940-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb940-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb940-179">Request</span></span>
<span data-ttu-id="eb940-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb940-180">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="eb940-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb940-181">Response</span></span>
<span data-ttu-id="eb940-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="eb940-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->