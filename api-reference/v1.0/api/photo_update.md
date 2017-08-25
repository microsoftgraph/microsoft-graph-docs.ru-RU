# <a name="update-photo"></a><span data-ttu-id="2218e-101">Обновление фотографии</span><span class="sxs-lookup"><span data-stu-id="2218e-101">Update photo</span></span>

<span data-ttu-id="2218e-102">Обновление свойств объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="2218e-102">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2218e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2218e-103">Permissions</span></span>
<span data-ttu-id="2218e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2218e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2218e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2218e-106">Permission type</span></span>      | <span data-ttu-id="2218e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2218e-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2218e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2218e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2218e-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2218e-109">Not supported.</span></span>    | 
|<span data-ttu-id="2218e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2218e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2218e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2218e-111">Not supported.</span></span>    | 
|<span data-ttu-id="2218e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2218e-112">Application</span></span> | <span data-ttu-id="2218e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2218e-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2218e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2218e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="2218e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2218e-115">Request headers</span></span>
| <span data-ttu-id="2218e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="2218e-116">Name</span></span>       | <span data-ttu-id="2218e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="2218e-117">Type</span></span> | <span data-ttu-id="2218e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2218e-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2218e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2218e-119">Authorization</span></span>  | <span data-ttu-id="2218e-120">string</span><span class="sxs-lookup"><span data-stu-id="2218e-120">string</span></span>  | <span data-ttu-id="2218e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2218e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2218e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2218e-123">Request body</span></span>
<span data-ttu-id="2218e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2218e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2218e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="2218e-127">Property</span></span>     | <span data-ttu-id="2218e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2218e-128">Type</span></span>   |<span data-ttu-id="2218e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2218e-129">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="2218e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2218e-130">Response</span></span>

<span data-ttu-id="2218e-131">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2218e-131">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2218e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2218e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2218e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2218e-133">Request</span></span>
<span data-ttu-id="2218e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2218e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="2218e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2218e-135">Response</span></span>
<span data-ttu-id="2218e-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2218e-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
