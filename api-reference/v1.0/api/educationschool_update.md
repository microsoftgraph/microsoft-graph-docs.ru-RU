# <a name="update-educationschool-properties"></a><span data-ttu-id="5a543-101">Обновление свойств educationSchool</span><span class="sxs-lookup"><span data-stu-id="5a543-101">Update educationschool properties</span></span>

<span data-ttu-id="5a543-102">Обновление свойств объекта school.</span><span class="sxs-lookup"><span data-stu-id="5a543-102">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a543-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a543-103">Permissions</span></span>
<span data-ttu-id="5a543-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a543-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a543-106">Permission type</span></span>      | <span data-ttu-id="5a543-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a543-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a543-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a543-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="5a543-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a543-109">Not supported.</span></span>  |
|<span data-ttu-id="5a543-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a543-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5a543-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a543-111">Not supported.</span></span>  |
|<span data-ttu-id="5a543-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a543-112">Application</span></span> | <span data-ttu-id="5a543-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a543-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a543-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a543-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5a543-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a543-115">Request headers</span></span>
| <span data-ttu-id="5a543-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a543-116">Header</span></span>       | <span data-ttu-id="5a543-117">Значение</span><span class="sxs-lookup"><span data-stu-id="5a543-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a543-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a543-118">Authorization</span></span>  | <span data-ttu-id="5a543-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a543-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a543-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a543-121">Content-Type</span></span>  | <span data-ttu-id="5a543-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a543-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a543-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a543-123">Request body</span></span>
<span data-ttu-id="5a543-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5a543-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5a543-125">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5a543-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5a543-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5a543-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a543-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a543-127">Property</span></span>     | <span data-ttu-id="5a543-128">Тип</span><span class="sxs-lookup"><span data-stu-id="5a543-128">Type</span></span>   |<span data-ttu-id="5a543-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5a543-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a543-130">displayName</span><span class="sxs-lookup"><span data-stu-id="5a543-130">displayName</span></span>| <span data-ttu-id="5a543-131">String</span><span class="sxs-lookup"><span data-stu-id="5a543-131">String</span></span>| <span data-ttu-id="5a543-132">Отображаемое имя школы</span><span class="sxs-lookup"><span data-stu-id="5a543-132">Display name of the school</span></span>| 
|<span data-ttu-id="5a543-133">description</span><span class="sxs-lookup"><span data-stu-id="5a543-133">description</span></span>| <span data-ttu-id="5a543-134">String</span><span class="sxs-lookup"><span data-stu-id="5a543-134">String</span></span> | <span data-ttu-id="5a543-135">Описание школы</span><span class="sxs-lookup"><span data-stu-id="5a543-135">Description of the school</span></span>| 
|<span data-ttu-id="5a543-136">principalEmail</span><span class="sxs-lookup"><span data-stu-id="5a543-136">principalEmail</span></span>| <span data-ttu-id="5a543-137">String</span><span class="sxs-lookup"><span data-stu-id="5a543-137">String</span></span>| <span data-ttu-id="5a543-138">Адрес электронной почты директора</span><span class="sxs-lookup"><span data-stu-id="5a543-138">Email address of the principal</span></span>|
|<span data-ttu-id="5a543-139">principalName</span><span class="sxs-lookup"><span data-stu-id="5a543-139">principalName</span></span>| <span data-ttu-id="5a543-140">String</span><span class="sxs-lookup"><span data-stu-id="5a543-140">String</span></span> | <span data-ttu-id="5a543-141">Имя директора</span><span class="sxs-lookup"><span data-stu-id="5a543-141">Name of the principal</span></span>|
|<span data-ttu-id="5a543-142">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="5a543-142">externalPrincipalId</span></span>| <span data-ttu-id="5a543-143">String</span><span class="sxs-lookup"><span data-stu-id="5a543-143">String</span></span> | <span data-ttu-id="5a543-144">Идентификатор директора в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5a543-144">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="5a543-145">highestGrade</span><span class="sxs-lookup"><span data-stu-id="5a543-145">highestGrade</span></span>|<span data-ttu-id="5a543-146">String</span><span class="sxs-lookup"><span data-stu-id="5a543-146">String</span></span>| <span data-ttu-id="5a543-147">Самый старший класс.</span><span class="sxs-lookup"><span data-stu-id="5a543-147">Highest grade taught.</span></span> |
|<span data-ttu-id="5a543-148">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="5a543-148">lowestGrade</span></span>|<span data-ttu-id="5a543-149">String</span><span class="sxs-lookup"><span data-stu-id="5a543-149">String</span></span>| <span data-ttu-id="5a543-150">Самый младший класс.</span><span class="sxs-lookup"><span data-stu-id="5a543-150">Lowest grade taught.</span></span> |
|<span data-ttu-id="5a543-151">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="5a543-151">schoolNumber</span></span>|<span data-ttu-id="5a543-152">String</span><span class="sxs-lookup"><span data-stu-id="5a543-152">String</span></span>| <span data-ttu-id="5a543-153">Номер школы.</span><span class="sxs-lookup"><span data-stu-id="5a543-153">School Number.</span></span>|
|<span data-ttu-id="5a543-154">externalId</span><span class="sxs-lookup"><span data-stu-id="5a543-154">externalId</span></span>|<span data-ttu-id="5a543-155">String</span><span class="sxs-lookup"><span data-stu-id="5a543-155">String</span></span>| <span data-ttu-id="5a543-156">Идентификатор учебного заведения в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5a543-156">Id of school in syncing system.</span></span> |
|<span data-ttu-id="5a543-157">phone</span><span class="sxs-lookup"><span data-stu-id="5a543-157">phone</span></span>|<span data-ttu-id="5a543-158">String</span><span class="sxs-lookup"><span data-stu-id="5a543-158">String</span></span>| <span data-ttu-id="5a543-159">Номер телефона учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a543-159">Phone number of school.</span></span> |
|<span data-ttu-id="5a543-160">fax</span><span class="sxs-lookup"><span data-stu-id="5a543-160">fax</span></span>|<span data-ttu-id="5a543-161">String</span><span class="sxs-lookup"><span data-stu-id="5a543-161">String</span></span>| <span data-ttu-id="5a543-162">Номер факса учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a543-162">Fax number of school.</span></span> |
|<span data-ttu-id="5a543-163">address</span><span class="sxs-lookup"><span data-stu-id="5a543-163">address</span></span>|[<span data-ttu-id="5a543-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5a543-164">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="5a543-165">Адрес учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="5a543-165">Address of the School.</span></span>|
|<span data-ttu-id="5a543-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a543-166">createdBy</span></span>|[<span data-ttu-id="5a543-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a543-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5a543-168">Объект, который создал учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="5a543-168">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="5a543-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a543-169">Response</span></span>
<span data-ttu-id="5a543-170">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a543-170">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a543-171">Пример</span><span class="sxs-lookup"><span data-stu-id="5a543-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a543-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a543-172">Request</span></span>
<span data-ttu-id="5a543-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a543-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="5a543-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a543-174">Response</span></span>
<span data-ttu-id="5a543-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a543-175">The following is an example of the response.</span></span> 

><span data-ttu-id="5a543-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a543-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
