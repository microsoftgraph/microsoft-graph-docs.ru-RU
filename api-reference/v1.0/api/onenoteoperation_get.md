# <a name="get-onenoteoperation"></a><span data-ttu-id="837e5-101">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="837e5-101">Get onenoteOperation</span></span>

<span data-ttu-id="837e5-p101">Получение сведений о состоянии операции OneNote, выполняющейся в течение длительного времени. Применяется к операциям, возвращающим заголовок **Operation-Location** в отклике, например `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="837e5-p101">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="837e5-104">Вы можете опрашивать конечную точку Operation-Location, пока свойство `status` не возвратит значение `completed` или `failed`.</span><span class="sxs-lookup"><span data-stu-id="837e5-104">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="837e5-105">Если операция имеет состояние `completed`, свойство `resourceLocation` содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="837e5-105">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="837e5-106">Если состояние `failed`, свойства `@api.diagnostics` и error предоставляют данные об ошибке.</span><span class="sxs-lookup"><span data-stu-id="837e5-106">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="837e5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="837e5-107">Permissions</span></span>
<span data-ttu-id="837e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="837e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="837e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="837e5-110">Permission type</span></span>      | <span data-ttu-id="837e5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="837e5-111">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="837e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="837e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="837e5-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837e5-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="837e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="837e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="837e5-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="837e5-115">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="837e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="837e5-116">Application</span></span> | <span data-ttu-id="837e5-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837e5-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="837e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="837e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="837e5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="837e5-119">Optional query parameters</span></span>
<span data-ttu-id="837e5-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="837e5-120">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="837e5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="837e5-121">Request headers</span></span>
| <span data-ttu-id="837e5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="837e5-122">Name</span></span>       | <span data-ttu-id="837e5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="837e5-123">Type</span></span> | <span data-ttu-id="837e5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="837e5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="837e5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="837e5-125">Authorization</span></span>  | <span data-ttu-id="837e5-126">string</span><span class="sxs-lookup"><span data-stu-id="837e5-126">string</span></span>  | <span data-ttu-id="837e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="837e5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="837e5-129">Accept</span><span class="sxs-lookup"><span data-stu-id="837e5-129">Accept</span></span> | <span data-ttu-id="837e5-130">строка</span><span class="sxs-lookup"><span data-stu-id="837e5-130">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="837e5-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="837e5-131">Request body</span></span>
<span data-ttu-id="837e5-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="837e5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="837e5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="837e5-133">Response</span></span>

<span data-ttu-id="837e5-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [onenoteOperation](../resources/onenoteoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="837e5-134">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="837e5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="837e5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="837e5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="837e5-136">Request</span></span>
<span data-ttu-id="837e5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="837e5-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="837e5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="837e5-138">Response</span></span>
<span data-ttu-id="837e5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="837e5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
