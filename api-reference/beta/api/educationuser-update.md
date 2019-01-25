---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: ae49192b349f39b091ecaa1706099e5f10782432
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517101"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="710b1-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="710b1-103">Update educationUser properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="710b1-104">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="710b1-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="710b1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="710b1-105">Permissions</span></span>
<span data-ttu-id="710b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="710b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="710b1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="710b1-108">Permission type</span></span>      | <span data-ttu-id="710b1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="710b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="710b1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="710b1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="710b1-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="710b1-111">Not supported.</span></span>  |
|<span data-ttu-id="710b1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="710b1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="710b1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="710b1-113">Not supported.</span></span>  |
|<span data-ttu-id="710b1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="710b1-114">Application</span></span> | <span data-ttu-id="710b1-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="710b1-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="710b1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="710b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="710b1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="710b1-117">Request headers</span></span>
| <span data-ttu-id="710b1-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="710b1-118">Header</span></span>       | <span data-ttu-id="710b1-119">Значение</span><span class="sxs-lookup"><span data-stu-id="710b1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="710b1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="710b1-120">Authorization</span></span>  | <span data-ttu-id="710b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="710b1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="710b1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="710b1-123">Content-Type</span></span>  | <span data-ttu-id="710b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="710b1-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="710b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="710b1-125">Request body</span></span>
<span data-ttu-id="710b1-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="710b1-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="710b1-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="710b1-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="710b1-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="710b1-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="710b1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="710b1-129">Property</span></span>     | <span data-ttu-id="710b1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="710b1-130">Type</span></span>   |<span data-ttu-id="710b1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="710b1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710b1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="710b1-132">displayName</span></span>| <span data-ttu-id="710b1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="710b1-133">String</span></span>| <span data-ttu-id="710b1-134">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="710b1-134">Display Name of User</span></span>|
|<span data-ttu-id="710b1-135">givenName</span><span class="sxs-lookup"><span data-stu-id="710b1-135">givenName</span></span>| <span data-ttu-id="710b1-136">String</span><span class="sxs-lookup"><span data-stu-id="710b1-136">String</span></span> | <span data-ttu-id="710b1-137">Имя</span><span class="sxs-lookup"><span data-stu-id="710b1-137">First Name</span></span> |
|<span data-ttu-id="710b1-138">middleName</span><span class="sxs-lookup"><span data-stu-id="710b1-138">middleName</span></span>| <span data-ttu-id="710b1-139">String</span><span class="sxs-lookup"><span data-stu-id="710b1-139">String</span></span> | <span data-ttu-id="710b1-140">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="710b1-140">Middle Name of user</span></span>|
|<span data-ttu-id="710b1-141">surname</span><span class="sxs-lookup"><span data-stu-id="710b1-141">surname</span></span>| <span data-ttu-id="710b1-142">String</span><span class="sxs-lookup"><span data-stu-id="710b1-142">String</span></span> | <span data-ttu-id="710b1-143">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="710b1-143">Surname of user</span></span>|
|<span data-ttu-id="710b1-144">mail</span><span class="sxs-lookup"><span data-stu-id="710b1-144">mail</span></span>| <span data-ttu-id="710b1-145">String</span><span class="sxs-lookup"><span data-stu-id="710b1-145">String</span></span>| <span data-ttu-id="710b1-146">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="710b1-146">email address</span></span>|
|<span data-ttu-id="710b1-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="710b1-147">mobilePhone</span></span>| <span data-ttu-id="710b1-148">String</span><span class="sxs-lookup"><span data-stu-id="710b1-148">String</span></span> | <span data-ttu-id="710b1-149">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="710b1-149">Mobile number of user</span></span> |
|<span data-ttu-id="710b1-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="710b1-150">externalSource</span></span>|<span data-ttu-id="710b1-151">string</span><span class="sxs-lookup"><span data-stu-id="710b1-151">string</span></span>| <span data-ttu-id="710b1-152">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="710b1-152">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="710b1-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="710b1-153">externalSource</span></span>|<span data-ttu-id="710b1-154">string</span><span class="sxs-lookup"><span data-stu-id="710b1-154">string</span></span>| <span data-ttu-id="710b1-155">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="710b1-155">Where this user was created from.</span></span>  <span data-ttu-id="710b1-156">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="710b1-156">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="710b1-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="710b1-157">mailingAddress</span></span>|[<span data-ttu-id="710b1-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="710b1-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="710b1-159">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="710b1-159">Mail address of user.</span></span>|
|<span data-ttu-id="710b1-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="710b1-160">residenceAddress</span></span>|[<span data-ttu-id="710b1-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="710b1-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="710b1-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="710b1-162">Address where user lives.</span></span>|
|<span data-ttu-id="710b1-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="710b1-163">primaryRole</span></span>|<span data-ttu-id="710b1-164">string</span><span class="sxs-lookup"><span data-stu-id="710b1-164">string</span></span>| <span data-ttu-id="710b1-165">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="710b1-165">Default Role for a user.</span></span>  <span data-ttu-id="710b1-166">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="710b1-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="710b1-167">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="710b1-167">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="710b1-168">student</span><span class="sxs-lookup"><span data-stu-id="710b1-168">student</span></span>|[<span data-ttu-id="710b1-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="710b1-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="710b1-170">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="710b1-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="710b1-171">teacher</span><span class="sxs-lookup"><span data-stu-id="710b1-171">teacher</span></span>|[<span data-ttu-id="710b1-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="710b1-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="710b1-173">Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.</span><span class="sxs-lookup"><span data-stu-id="710b1-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="710b1-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="710b1-174">Response</span></span>
<span data-ttu-id="710b1-175">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="710b1-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="710b1-176">Пример</span><span class="sxs-lookup"><span data-stu-id="710b1-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="710b1-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="710b1-177">Request</span></span>
<span data-ttu-id="710b1-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="710b1-178">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="710b1-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="710b1-179">Response</span></span>
<span data-ttu-id="710b1-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="710b1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/educationuser-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
