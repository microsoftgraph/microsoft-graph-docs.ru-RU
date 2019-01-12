---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 52b9e3f3784bae75ed9a2d4aa91fc52dd8917de6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976186"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="4d989-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="4d989-103">Update educationUser properties</span></span>

> <span data-ttu-id="4d989-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d989-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d989-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d989-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d989-106">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="4d989-106">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d989-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d989-107">Permissions</span></span>
<span data-ttu-id="4d989-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d989-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d989-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d989-110">Permission type</span></span>      | <span data-ttu-id="4d989-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d989-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d989-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d989-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4d989-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d989-113">Not supported.</span></span>  |
|<span data-ttu-id="4d989-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d989-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4d989-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d989-115">Not supported.</span></span>  |
|<span data-ttu-id="4d989-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d989-116">Application</span></span> | <span data-ttu-id="4d989-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d989-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d989-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d989-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4d989-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d989-119">Request headers</span></span>
| <span data-ttu-id="4d989-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d989-120">Header</span></span>       | <span data-ttu-id="4d989-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4d989-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d989-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d989-122">Authorization</span></span>  | <span data-ttu-id="4d989-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d989-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4d989-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d989-125">Content-Type</span></span>  | <span data-ttu-id="4d989-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d989-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d989-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d989-127">Request body</span></span>
<span data-ttu-id="4d989-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4d989-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4d989-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4d989-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4d989-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4d989-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4d989-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d989-131">Property</span></span>     | <span data-ttu-id="4d989-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4d989-132">Type</span></span>   |<span data-ttu-id="4d989-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4d989-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d989-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4d989-134">displayName</span></span>| <span data-ttu-id="4d989-135">String</span><span class="sxs-lookup"><span data-stu-id="4d989-135">String</span></span>| <span data-ttu-id="4d989-136">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="4d989-136">Display Name of User</span></span>|
|<span data-ttu-id="4d989-137">givenName</span><span class="sxs-lookup"><span data-stu-id="4d989-137">givenName</span></span>| <span data-ttu-id="4d989-138">String</span><span class="sxs-lookup"><span data-stu-id="4d989-138">String</span></span> | <span data-ttu-id="4d989-139">Имя</span><span class="sxs-lookup"><span data-stu-id="4d989-139">First Name</span></span> |
|<span data-ttu-id="4d989-140">middleName</span><span class="sxs-lookup"><span data-stu-id="4d989-140">middleName</span></span>| <span data-ttu-id="4d989-141">String</span><span class="sxs-lookup"><span data-stu-id="4d989-141">String</span></span> | <span data-ttu-id="4d989-142">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="4d989-142">Middle Name of user</span></span>|
|<span data-ttu-id="4d989-143">surname</span><span class="sxs-lookup"><span data-stu-id="4d989-143">surname</span></span>| <span data-ttu-id="4d989-144">String</span><span class="sxs-lookup"><span data-stu-id="4d989-144">String</span></span> | <span data-ttu-id="4d989-145">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="4d989-145">Surname of user</span></span>|
|<span data-ttu-id="4d989-146">mail</span><span class="sxs-lookup"><span data-stu-id="4d989-146">mail</span></span>| <span data-ttu-id="4d989-147">String</span><span class="sxs-lookup"><span data-stu-id="4d989-147">String</span></span>| <span data-ttu-id="4d989-148">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="4d989-148">email address</span></span>|
|<span data-ttu-id="4d989-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="4d989-149">mobilePhone</span></span>| <span data-ttu-id="4d989-150">String</span><span class="sxs-lookup"><span data-stu-id="4d989-150">String</span></span> | <span data-ttu-id="4d989-151">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="4d989-151">Mobile number of user</span></span> |
|<span data-ttu-id="4d989-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="4d989-152">externalSource</span></span>|<span data-ttu-id="4d989-153">строка</span><span class="sxs-lookup"><span data-stu-id="4d989-153">string</span></span>| <span data-ttu-id="4d989-154">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="4d989-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="4d989-155">externalSource</span><span class="sxs-lookup"><span data-stu-id="4d989-155">externalSource</span></span>|<span data-ttu-id="4d989-156">строка</span><span class="sxs-lookup"><span data-stu-id="4d989-156">string</span></span>| <span data-ttu-id="4d989-157">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d989-157">Where this user was created from.</span></span>  <span data-ttu-id="4d989-158">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="4d989-158">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="4d989-159">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="4d989-159">mailingAddress</span></span>|[<span data-ttu-id="4d989-160">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4d989-160">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="4d989-161">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d989-161">Mail address of user.</span></span>|
|<span data-ttu-id="4d989-162">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="4d989-162">residenceAddress</span></span>|[<span data-ttu-id="4d989-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4d989-163">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="4d989-164">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d989-164">Address where user lives.</span></span>|
|<span data-ttu-id="4d989-165">primaryRole</span><span class="sxs-lookup"><span data-stu-id="4d989-165">primaryRole</span></span>|<span data-ttu-id="4d989-166">строка</span><span class="sxs-lookup"><span data-stu-id="4d989-166">string</span></span>| <span data-ttu-id="4d989-167">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d989-167">Default Role for a user.</span></span>  <span data-ttu-id="4d989-168">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="4d989-168">The user's role might be different in an individual class.</span></span> <span data-ttu-id="4d989-169">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="4d989-169">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="4d989-170">student</span><span class="sxs-lookup"><span data-stu-id="4d989-170">student</span></span>|[<span data-ttu-id="4d989-171">educationStudent</span><span class="sxs-lookup"><span data-stu-id="4d989-171">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="4d989-172">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="4d989-172">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="4d989-173">teacher</span><span class="sxs-lookup"><span data-stu-id="4d989-173">teacher</span></span>|[<span data-ttu-id="4d989-174">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="4d989-174">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="4d989-175">Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.</span><span class="sxs-lookup"><span data-stu-id="4d989-175">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="4d989-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d989-176">Response</span></span>
<span data-ttu-id="4d989-177">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4d989-177">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d989-178">Пример</span><span class="sxs-lookup"><span data-stu-id="4d989-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d989-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d989-179">Request</span></span>
<span data-ttu-id="4d989-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d989-180">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4d989-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d989-181">Response</span></span>
<span data-ttu-id="4d989-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4d989-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
