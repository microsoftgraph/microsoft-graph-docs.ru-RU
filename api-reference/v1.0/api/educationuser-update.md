---
title: Обновление свойств educationUser
description: Обновление свойств объекта **educationuser**.
localization_priority: Normal
ms.openlocfilehash: aef8640f49ad6ff4d91755fd5200000f4a0e856d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856660"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="01222-103">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="01222-103">Update educationUser properties</span></span>

<span data-ttu-id="01222-104">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="01222-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="01222-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01222-105">Permissions</span></span>
<span data-ttu-id="01222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01222-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01222-108">Permission type</span></span>      | <span data-ttu-id="01222-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01222-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01222-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01222-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="01222-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01222-111">Not supported.</span></span>  |
|<span data-ttu-id="01222-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01222-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="01222-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01222-113">Not supported.</span></span>  |
|<span data-ttu-id="01222-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01222-114">Application</span></span> | <span data-ttu-id="01222-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01222-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01222-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01222-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="01222-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01222-117">Request headers</span></span>
| <span data-ttu-id="01222-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01222-118">Header</span></span>       | <span data-ttu-id="01222-119">Значение</span><span class="sxs-lookup"><span data-stu-id="01222-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01222-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01222-120">Authorization</span></span>  | <span data-ttu-id="01222-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01222-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01222-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01222-123">Content-Type</span></span>  | <span data-ttu-id="01222-124">application/json</span><span class="sxs-lookup"><span data-stu-id="01222-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01222-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01222-125">Request body</span></span>
<span data-ttu-id="01222-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="01222-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="01222-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="01222-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="01222-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="01222-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="01222-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01222-129">Property</span></span>     | <span data-ttu-id="01222-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01222-130">Type</span></span>   |<span data-ttu-id="01222-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01222-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01222-132">displayName</span><span class="sxs-lookup"><span data-stu-id="01222-132">displayName</span></span>| <span data-ttu-id="01222-133">String</span><span class="sxs-lookup"><span data-stu-id="01222-133">String</span></span>| <span data-ttu-id="01222-134">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="01222-134">Display Name of User</span></span>|
|<span data-ttu-id="01222-135">givenName</span><span class="sxs-lookup"><span data-stu-id="01222-135">givenName</span></span>| <span data-ttu-id="01222-136">String</span><span class="sxs-lookup"><span data-stu-id="01222-136">String</span></span> | <span data-ttu-id="01222-137">Имя</span><span class="sxs-lookup"><span data-stu-id="01222-137">First Name</span></span> |
|<span data-ttu-id="01222-138">middleName</span><span class="sxs-lookup"><span data-stu-id="01222-138">middleName</span></span>| <span data-ttu-id="01222-139">String</span><span class="sxs-lookup"><span data-stu-id="01222-139">String</span></span> | <span data-ttu-id="01222-140">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="01222-140">Middle Name of user</span></span>|
|<span data-ttu-id="01222-141">surname</span><span class="sxs-lookup"><span data-stu-id="01222-141">surname</span></span>| <span data-ttu-id="01222-142">String</span><span class="sxs-lookup"><span data-stu-id="01222-142">String</span></span> | <span data-ttu-id="01222-143">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="01222-143">Surname of user</span></span>|
|<span data-ttu-id="01222-144">mail</span><span class="sxs-lookup"><span data-stu-id="01222-144">mail</span></span>| <span data-ttu-id="01222-145">String</span><span class="sxs-lookup"><span data-stu-id="01222-145">String</span></span>| <span data-ttu-id="01222-146">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="01222-146">email address</span></span>|
|<span data-ttu-id="01222-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="01222-147">mobilePhone</span></span>| <span data-ttu-id="01222-148">String</span><span class="sxs-lookup"><span data-stu-id="01222-148">String</span></span> | <span data-ttu-id="01222-149">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="01222-149">Mobile number of user</span></span> |
|<span data-ttu-id="01222-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="01222-150">externalSource</span></span>|<span data-ttu-id="01222-151">string</span><span class="sxs-lookup"><span data-stu-id="01222-151">string</span></span>| <span data-ttu-id="01222-152">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="01222-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="01222-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="01222-153">externalSource</span></span>|<span data-ttu-id="01222-154">string</span><span class="sxs-lookup"><span data-stu-id="01222-154">string</span></span>| <span data-ttu-id="01222-155">Источник для создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="01222-155">Where this user was created from.</span></span>  <span data-ttu-id="01222-156">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="01222-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="01222-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="01222-157">mailingAddress</span></span>|[<span data-ttu-id="01222-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="01222-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="01222-159">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="01222-159">Mail address of user.</span></span>|
|<span data-ttu-id="01222-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="01222-160">residenceAddress</span></span>|[<span data-ttu-id="01222-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="01222-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="01222-162">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="01222-162">Address where user lives.</span></span>|
|<span data-ttu-id="01222-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="01222-163">primaryRole</span></span>|<span data-ttu-id="01222-164">string</span><span class="sxs-lookup"><span data-stu-id="01222-164">string</span></span>| <span data-ttu-id="01222-165">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="01222-165">Default Role for a user.</span></span>  <span data-ttu-id="01222-166">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="01222-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="01222-167">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="01222-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="01222-168">student</span><span class="sxs-lookup"><span data-stu-id="01222-168">student</span></span>|[<span data-ttu-id="01222-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="01222-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="01222-170">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="01222-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="01222-171">teacher</span><span class="sxs-lookup"><span data-stu-id="01222-171">teacher</span></span>|[<span data-ttu-id="01222-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="01222-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="01222-173">Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.</span><span class="sxs-lookup"><span data-stu-id="01222-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="01222-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="01222-174">Response</span></span>
<span data-ttu-id="01222-175">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01222-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01222-176">Пример</span><span class="sxs-lookup"><span data-stu-id="01222-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01222-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="01222-177">Request</span></span>
<span data-ttu-id="01222-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01222-178">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="01222-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="01222-179">Response</span></span>
<span data-ttu-id="01222-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01222-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
