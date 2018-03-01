# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="0c02b-101">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="0c02b-101">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="0c02b-102">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="0c02b-102">Add a user to a role</span></span>

## <a name="permissions"></a><span data-ttu-id="0c02b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c02b-103">Permissions</span></span>
<span data-ttu-id="0c02b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c02b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c02b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c02b-106">Permission type</span></span>      | <span data-ttu-id="0c02b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c02b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c02b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c02b-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c02b-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c02b-109">Not supported.</span></span>  |
|<span data-ttu-id="0c02b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c02b-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c02b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c02b-111">Not supported.</span></span>  |
|<span data-ttu-id="0c02b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c02b-112">Application</span></span> | <span data-ttu-id="0c02b-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c02b-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c02b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c02b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0c02b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c02b-115">Request headers</span></span>
| <span data-ttu-id="0c02b-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c02b-116">Header</span></span>       | <span data-ttu-id="0c02b-117">Значение</span><span class="sxs-lookup"><span data-stu-id="0c02b-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c02b-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c02b-118">Authorization</span></span>  | <span data-ttu-id="0c02b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c02b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c02b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c02b-121">Content-Type</span></span>  | <span data-ttu-id="0c02b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0c02b-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c02b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c02b-123">Request body</span></span>
<span data-ttu-id="0c02b-124">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c02b-124">In the request body, supply a JSON representation of an [invitation](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0c02b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c02b-125">Response</span></span>
<span data-ttu-id="0c02b-126">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c02b-126">If successful, this method returns a `204 No Content` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c02b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0c02b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c02b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c02b-128">Request</span></span>
<span data-ttu-id="0c02b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c02b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/<id>/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="0c02b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c02b-130">Response</span></span>
<span data-ttu-id="0c02b-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0c02b-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->