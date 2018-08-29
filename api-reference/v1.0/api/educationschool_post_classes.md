# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="32d8b-101">Добавление educationClass к educationSchool</span><span class="sxs-lookup"><span data-stu-id="32d8b-101">Add educationClass to educationSchool</span></span>

<span data-ttu-id="32d8b-102">Добавление класса в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="32d8b-102">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="32d8b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32d8b-103">Permissions</span></span>
<span data-ttu-id="32d8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32d8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32d8b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32d8b-106">Permission type</span></span>      | <span data-ttu-id="32d8b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32d8b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32d8b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32d8b-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="32d8b-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32d8b-109">Not supported.</span></span>  |
|<span data-ttu-id="32d8b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32d8b-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="32d8b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32d8b-111">Not supported.</span></span>  |
|<span data-ttu-id="32d8b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32d8b-112">Application</span></span> | <span data-ttu-id="32d8b-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d8b-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="32d8b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32d8b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="32d8b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32d8b-115">Request headers</span></span>
| <span data-ttu-id="32d8b-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32d8b-116">Header</span></span>       | <span data-ttu-id="32d8b-117">Значение</span><span class="sxs-lookup"><span data-stu-id="32d8b-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32d8b-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32d8b-118">Authorization</span></span>  | <span data-ttu-id="32d8b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32d8b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="32d8b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32d8b-121">Content-Type</span></span>  | <span data-ttu-id="32d8b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="32d8b-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32d8b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32d8b-123">Request body</span></span>
<span data-ttu-id="32d8b-124">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32d8b-124">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="32d8b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="32d8b-125">Response</span></span>
<span data-ttu-id="32d8b-126">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32d8b-126">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32d8b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="32d8b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32d8b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="32d8b-128">Request</span></span>
<span data-ttu-id="32d8b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32d8b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="32d8b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="32d8b-130">Response</span></span> 
<span data-ttu-id="32d8b-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="32d8b-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->