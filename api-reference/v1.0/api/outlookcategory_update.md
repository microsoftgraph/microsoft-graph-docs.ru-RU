# <a name="update-outlook-category"></a><span data-ttu-id="1d94f-101">Обновление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="1d94f-101">Update Outlook category</span></span>


<span data-ttu-id="1d94f-102">Обновление перезаписываемого свойства **color** указанного объекта [outlookCategory](../resources/outlookCategory.md).</span><span class="sxs-lookup"><span data-stu-id="1d94f-102">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span> <span data-ttu-id="1d94f-103">Нельзя изменить свойство **displayName** после создания категории.</span><span class="sxs-lookup"><span data-stu-id="1d94f-103">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d94f-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d94f-104">Permissions</span></span>
<span data-ttu-id="1d94f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d94f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d94f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d94f-107">Permission type</span></span>      | <span data-ttu-id="1d94f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d94f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d94f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d94f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1d94f-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d94f-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1d94f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d94f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d94f-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d94f-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1d94f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d94f-113">Application</span></span> | <span data-ttu-id="1d94f-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d94f-114">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d94f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d94f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d94f-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d94f-116">Optional query parameters</span></span>
<span data-ttu-id="1d94f-117">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1d94f-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d94f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d94f-118">Request headers</span></span>
| <span data-ttu-id="1d94f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1d94f-119">Name</span></span>      |<span data-ttu-id="1d94f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1d94f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d94f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d94f-121">Authorization</span></span>  | <span data-ttu-id="1d94f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d94f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d94f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d94f-124">Request body</span></span>
<span data-ttu-id="1d94f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1d94f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d94f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d94f-128">Property</span></span>     | <span data-ttu-id="1d94f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1d94f-129">Type</span></span>   |<span data-ttu-id="1d94f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1d94f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d94f-131">color</span><span class="sxs-lookup"><span data-stu-id="1d94f-131">color</span></span>|<span data-ttu-id="1d94f-132">String</span><span class="sxs-lookup"><span data-stu-id="1d94f-132">String</span></span>|<span data-ttu-id="1d94f-133">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="1d94f-133">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="1d94f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d94f-134">Response</span></span>

<span data-ttu-id="1d94f-135">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [outlookCategory](../resources/outlookCategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1d94f-135">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookCategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d94f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1d94f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d94f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d94f-137">Request</span></span>
<span data-ttu-id="1d94f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d94f-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="1d94f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d94f-139">Response</span></span>
<span data-ttu-id="1d94f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d94f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->