# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="36974-101">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="36974-101">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="36974-102">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="36974-102">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="36974-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36974-103">Permissions</span></span>
<span data-ttu-id="36974-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="36974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="36974-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36974-106">Permission type</span></span>      | <span data-ttu-id="36974-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36974-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36974-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36974-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="36974-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36974-109">Not supported.</span></span>  |
|<span data-ttu-id="36974-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36974-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36974-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36974-111">Not supported.</span></span>  |
|<span data-ttu-id="36974-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36974-112">Application</span></span> | <span data-ttu-id="36974-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36974-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36974-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36974-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/<id>/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="36974-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36974-115">Request headers</span></span>
| <span data-ttu-id="36974-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36974-116">Header</span></span>       | <span data-ttu-id="36974-117">Значение</span><span class="sxs-lookup"><span data-stu-id="36974-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36974-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36974-118">Authorization</span></span>  | <span data-ttu-id="36974-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36974-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36974-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36974-121">Request body</span></span>
<span data-ttu-id="36974-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36974-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="36974-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="36974-123">Response</span></span>
<span data-ttu-id="36974-124">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="36974-124">If successful, this method returns a `204 No Content` response code and an event object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36974-125">Пример</span><span class="sxs-lookup"><span data-stu-id="36974-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36974-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="36974-126">Request</span></span>
<span data-ttu-id="36974-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36974-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/10001/users/13006
```

##### <a name="response"></a><span data-ttu-id="36974-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="36974-128">Response</span></span>
<span data-ttu-id="36974-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36974-129">The following is an example of the response.</span></span> 
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