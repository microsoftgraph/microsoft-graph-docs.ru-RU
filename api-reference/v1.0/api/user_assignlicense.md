# <a name="assignlicense"></a><span data-ttu-id="9ea1f-101">assignLicense</span><span class="sxs-lookup"><span data-stu-id="9ea1f-101">assignLicense</span></span>
<span data-ttu-id="9ea1f-p101">Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-p101">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea1f-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea1f-104">Permissions</span></span>
<span data-ttu-id="9ea1f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ea1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ea1f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea1f-107">Permission type</span></span>      | <span data-ttu-id="9ea1f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ea1f-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9ea1f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ea1f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9ea1f-110">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea1f-110">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    | 
|<span data-ttu-id="9ea1f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ea1f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea1f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-112">Not supported.</span></span>    | 
|<span data-ttu-id="9ea1f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ea1f-113">Application</span></span> | <span data-ttu-id="9ea1f-114">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea1f-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9ea1f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ea1f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="9ea1f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ea1f-116">Request headers</span></span>
| <span data-ttu-id="9ea1f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ea1f-117">Header</span></span>       | <span data-ttu-id="9ea1f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9ea1f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ea1f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ea1f-119">Authorization</span></span>  | <span data-ttu-id="9ea1f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ea1f-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ea1f-122">Content-Type</span></span>  | <span data-ttu-id="9ea1f-123">application/json</span><span class="sxs-lookup"><span data-stu-id="9ea1f-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ea1f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ea1f-124">Request body</span></span>
<span data-ttu-id="9ea1f-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ea1f-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ea1f-126">Parameter</span></span>    | <span data-ttu-id="9ea1f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9ea1f-127">Type</span></span>   |<span data-ttu-id="9ea1f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9ea1f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ea1f-129">addLicenses</span><span class="sxs-lookup"><span data-stu-id="9ea1f-129">addLicenses</span></span>|<span data-ttu-id="9ea1f-130">AssignedLicense</span><span class="sxs-lookup"><span data-stu-id="9ea1f-130">AssignedLicense</span></span>|<span data-ttu-id="9ea1f-p104">Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии. Вы можете отключить планы, связанные с лицензией, задав свойство **disabledPlans** объекта [assignedLicense](../resources/assignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="9ea1f-p104">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="9ea1f-133">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="9ea1f-133">removeLicenses</span></span>|<span data-ttu-id="9ea1f-134">Guid</span><span class="sxs-lookup"><span data-stu-id="9ea1f-134">Guid</span></span>|<span data-ttu-id="9ea1f-135">Коллекция идентификаторов GUID, указывающих удаляемые лицензии.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-135">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="9ea1f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea1f-136">Response</span></span>

<span data-ttu-id="9ea1f-137">В случае успеха этот метод возвращает код отклика `200, OK` и объект [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-137">If successful, this method returns `200, OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea1f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9ea1f-138">Example</span></span>
<span data-ttu-id="9ea1f-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ea1f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ea1f-140">Request</span></span>
<span data-ttu-id="9ea1f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="9ea1f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ea1f-142">Response</span></span>
<span data-ttu-id="9ea1f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9ea1f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
