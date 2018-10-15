# <a name="update-educationuser-properties"></a><span data-ttu-id="3e4d4-101">Обновление свойств educationUser</span><span class="sxs-lookup"><span data-stu-id="3e4d4-101">Update educationUser properties</span></span>

<span data-ttu-id="3e4d4-102">Обновление свойств объекта **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-102">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e4d4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4d4-103">Permissions</span></span>
<span data-ttu-id="3e4d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e4d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e4d4-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4d4-106">Permission type</span></span>      | <span data-ttu-id="3e4d4-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e4d4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e4d4-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e4d4-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="3e4d4-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-109">Not supported.</span></span>  |
|<span data-ttu-id="3e4d4-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e4d4-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3e4d4-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-111">Not supported.</span></span>  |
|<span data-ttu-id="3e4d4-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e4d4-112">Application</span></span> | <span data-ttu-id="3e4d4-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4d4-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e4d4-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e4d4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3e4d4-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e4d4-115">Request headers</span></span>
| <span data-ttu-id="3e4d4-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e4d4-116">Header</span></span>       | <span data-ttu-id="3e4d4-117">Значение</span><span class="sxs-lookup"><span data-stu-id="3e4d4-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e4d4-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e4d4-118">Authorization</span></span>  | <span data-ttu-id="3e4d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e4d4-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e4d4-121">Content-Type</span></span>  | <span data-ttu-id="3e4d4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3e4d4-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e4d4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e4d4-123">Request body</span></span>
<span data-ttu-id="3e4d4-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3e4d4-125">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3e4d4-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e4d4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e4d4-127">Property</span></span>     | <span data-ttu-id="3e4d4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3e4d4-128">Type</span></span>   |<span data-ttu-id="3e4d4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3e4d4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e4d4-130">displayName</span><span class="sxs-lookup"><span data-stu-id="3e4d4-130">displayName</span></span>| <span data-ttu-id="3e4d4-131">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4d4-131">String</span></span>| <span data-ttu-id="3e4d4-132">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="3e4d4-132">Display Name of User</span></span>|
|<span data-ttu-id="3e4d4-133">givenName</span><span class="sxs-lookup"><span data-stu-id="3e4d4-133">givenName</span></span>| <span data-ttu-id="3e4d4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4d4-134">String</span></span> | <span data-ttu-id="3e4d4-135">Имя</span><span class="sxs-lookup"><span data-stu-id="3e4d4-135">First Name</span></span> |
|<span data-ttu-id="3e4d4-136">middleName</span><span class="sxs-lookup"><span data-stu-id="3e4d4-136">middleName</span></span>| <span data-ttu-id="3e4d4-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4d4-137">String</span></span> | <span data-ttu-id="3e4d4-138">Отчество пользователя</span><span class="sxs-lookup"><span data-stu-id="3e4d4-138">Middle Name of user</span></span>|
|<span data-ttu-id="3e4d4-139">surname</span><span class="sxs-lookup"><span data-stu-id="3e4d4-139">surname</span></span>| <span data-ttu-id="3e4d4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4d4-140">String</span></span> | <span data-ttu-id="3e4d4-141">Фамилия пользователя</span><span class="sxs-lookup"><span data-stu-id="3e4d4-141">Surname of user</span></span>|
|<span data-ttu-id="3e4d4-142">mail</span><span class="sxs-lookup"><span data-stu-id="3e4d4-142">mail</span></span>| <span data-ttu-id="3e4d4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4d4-143">String</span></span>| <span data-ttu-id="3e4d4-144">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="3e4d4-144">email address</span></span>|
|<span data-ttu-id="3e4d4-145">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="3e4d4-145">mobilePhone</span></span>| <span data-ttu-id="3e4d4-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3e4d4-146">String</span></span> | <span data-ttu-id="3e4d4-147">Номер мобильного телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="3e4d4-147">Mobile number of user</span></span> |
|<span data-ttu-id="3e4d4-148">externalSource</span><span class="sxs-lookup"><span data-stu-id="3e4d4-148">externalSource</span></span>|<span data-ttu-id="3e4d4-149">Cтрока</span><span class="sxs-lookup"><span data-stu-id="3e4d4-149">string</span></span>| <span data-ttu-id="3e4d4-150">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-150">The possible values are `sis`, `manual`, `enum_sentinel`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="3e4d4-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="3e4d4-151">externalSource</span></span>|<span data-ttu-id="3e4d4-152">Cтрока</span><span class="sxs-lookup"><span data-stu-id="3e4d4-152">string</span></span>| <span data-ttu-id="3e4d4-153">Источник создания пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-153">Where this user was created from.</span></span>  <span data-ttu-id="3e4d4-154">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-154">The possible values are `sis`, `manual`, `enum_sentinel`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="3e4d4-155">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="3e4d4-155">mailingAddress</span></span>|[<span data-ttu-id="3e4d4-156">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3e4d4-156">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="3e4d4-157">Почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-157">Mail address of user.</span></span>|
|<span data-ttu-id="3e4d4-158">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="3e4d4-158">residenceAddress</span></span>|[<span data-ttu-id="3e4d4-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3e4d4-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="3e4d4-160">Адрес проживания пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-160">Address where user lives.</span></span>|
|<span data-ttu-id="3e4d4-161">primaryRole</span><span class="sxs-lookup"><span data-stu-id="3e4d4-161">primaryRole</span></span>|<span data-ttu-id="3e4d4-162">Cтрока</span><span class="sxs-lookup"><span data-stu-id="3e4d4-162">string</span></span>| <span data-ttu-id="3e4d4-163">Роль по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-163">Default Role for a user.</span></span>  <span data-ttu-id="3e4d4-164">Роль пользователя для отдельного курса может отличаться.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-164">The user's role might be different in an individual class.</span></span> <span data-ttu-id="3e4d4-165">Возможные значения: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-165">The possible values are `student`, `teacher`, `enum_sentinel`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="3e4d4-166">student</span><span class="sxs-lookup"><span data-stu-id="3e4d4-166">student</span></span>|[<span data-ttu-id="3e4d4-167">educationStudent</span><span class="sxs-lookup"><span data-stu-id="3e4d4-167">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="3e4d4-168">Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-168">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="3e4d4-169">teacher</span><span class="sxs-lookup"><span data-stu-id="3e4d4-169">teacher</span></span>|[<span data-ttu-id="3e4d4-170">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="3e4d4-170">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="3e4d4-171">Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-171">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="3e4d4-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e4d4-172">Response</span></span>
<span data-ttu-id="3e4d4-173">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-173">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e4d4-174">Пример</span><span class="sxs-lookup"><span data-stu-id="3e4d4-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e4d4-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e4d4-175">Request</span></span>
<span data-ttu-id="3e4d4-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-176">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3e4d4-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e4d4-177">Response</span></span>
<span data-ttu-id="3e4d4-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e4d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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