# <a name="update-mailfolder"></a><span data-ttu-id="95d16-101">Обновление объекта mailfolder</span><span class="sxs-lookup"><span data-stu-id="95d16-101">Update mailfolder</span></span>

<span data-ttu-id="95d16-102">Обновление свойств объекта mailfolder.</span><span class="sxs-lookup"><span data-stu-id="95d16-102">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="95d16-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95d16-103">Permissions</span></span>
<span data-ttu-id="95d16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95d16-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95d16-106">Permission type</span></span>      | <span data-ttu-id="95d16-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95d16-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="95d16-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95d16-108">Delegated (work or school account)</span></span> | <span data-ttu-id="95d16-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95d16-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="95d16-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95d16-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95d16-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95d16-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="95d16-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95d16-112">Application</span></span> | <span data-ttu-id="95d16-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95d16-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="95d16-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95d16-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="95d16-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95d16-115">Request headers</span></span>
| <span data-ttu-id="95d16-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95d16-116">Header</span></span>       | <span data-ttu-id="95d16-117">Значение</span><span class="sxs-lookup"><span data-stu-id="95d16-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95d16-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95d16-118">Authorization</span></span>  | <span data-ttu-id="95d16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d16-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95d16-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95d16-121">Content-Type</span></span>  | <span data-ttu-id="95d16-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d16-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95d16-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95d16-124">Request body</span></span>
<span data-ttu-id="95d16-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="95d16-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="95d16-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="95d16-128">Property</span></span>     | <span data-ttu-id="95d16-129">Тип</span><span class="sxs-lookup"><span data-stu-id="95d16-129">Type</span></span>   |<span data-ttu-id="95d16-130">Описание</span><span class="sxs-lookup"><span data-stu-id="95d16-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95d16-131">displayName</span><span class="sxs-lookup"><span data-stu-id="95d16-131">displayName</span></span>|<span data-ttu-id="95d16-132">Строка</span><span class="sxs-lookup"><span data-stu-id="95d16-132">String</span></span>|<span data-ttu-id="95d16-133">Отображаемое имя объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="95d16-133">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="95d16-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d16-134">Response</span></span>

<span data-ttu-id="95d16-135">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95d16-135">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95d16-136">Пример</span><span class="sxs-lookup"><span data-stu-id="95d16-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95d16-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="95d16-137">Request</span></span>
<span data-ttu-id="95d16-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95d16-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="95d16-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="95d16-139">Response</span></span>
<span data-ttu-id="95d16-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="95d16-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
