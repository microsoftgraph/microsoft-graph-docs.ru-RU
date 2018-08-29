# <a name="remove-teacher"></a><span data-ttu-id="32c1e-101">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="32c1e-101">Remove teacher</span></span>

<span data-ttu-id="32c1e-102">Удаление преподавателя для курса.</span><span class="sxs-lookup"><span data-stu-id="32c1e-102">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="32c1e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32c1e-103">Permissions</span></span>
<span data-ttu-id="32c1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32c1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32c1e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32c1e-106">Permission type</span></span>      | <span data-ttu-id="32c1e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32c1e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32c1e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32c1e-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="32c1e-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32c1e-109">Not supported.</span></span>  |
|<span data-ttu-id="32c1e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32c1e-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="32c1e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32c1e-111">Not supported.</span></span>  |
|<span data-ttu-id="32c1e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32c1e-112">Application</span></span> | <span data-ttu-id="32c1e-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c1e-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="32c1e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32c1e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="32c1e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32c1e-115">Request headers</span></span>
| <span data-ttu-id="32c1e-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32c1e-116">Header</span></span>       | <span data-ttu-id="32c1e-117">Значение</span><span class="sxs-lookup"><span data-stu-id="32c1e-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32c1e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32c1e-118">Authorization</span></span>  | <span data-ttu-id="32c1e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32c1e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32c1e-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32c1e-121">Request body</span></span>
<span data-ttu-id="32c1e-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32c1e-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="32c1e-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="32c1e-123">Response</span></span>
<span data-ttu-id="32c1e-124">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="32c1e-124">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="32c1e-125">Пример</span><span class="sxs-lookup"><span data-stu-id="32c1e-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32c1e-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="32c1e-126">Request</span></span>
<span data-ttu-id="32c1e-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32c1e-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="32c1e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="32c1e-128">Response</span></span>
<span data-ttu-id="32c1e-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="32c1e-129">The following is an example of the response.</span></span> 
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
