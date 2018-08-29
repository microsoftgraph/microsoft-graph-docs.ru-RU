# <a name="remove-educationclass"></a><span data-ttu-id="b9140-101">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="b9140-101">Remove educationClass</span></span>

<span data-ttu-id="b9140-102">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="b9140-102">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9140-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9140-103">Permissions</span></span>
<span data-ttu-id="b9140-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9140-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9140-106">Permission type</span></span>      | <span data-ttu-id="b9140-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9140-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9140-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9140-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9140-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9140-109">Not supported.</span></span>  |
|<span data-ttu-id="b9140-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9140-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b9140-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9140-111">Not supported.</span></span>  |
|<span data-ttu-id="b9140-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9140-112">Application</span></span> | <span data-ttu-id="b9140-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9140-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9140-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9140-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b9140-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9140-115">Request headers</span></span>
| <span data-ttu-id="b9140-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9140-116">Header</span></span>       | <span data-ttu-id="b9140-117">Значение</span><span class="sxs-lookup"><span data-stu-id="b9140-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9140-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9140-118">Authorization</span></span>  | <span data-ttu-id="b9140-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9140-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9140-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9140-121">Request body</span></span>
<span data-ttu-id="b9140-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9140-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b9140-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9140-123">Response</span></span>
<span data-ttu-id="b9140-124">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="b9140-124">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9140-125">Пример</span><span class="sxs-lookup"><span data-stu-id="b9140-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9140-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9140-126">Request</span></span>
<span data-ttu-id="b9140-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9140-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="b9140-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9140-128">Response</span></span>
<span data-ttu-id="b9140-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b9140-129">The following is an example of the response.</span></span> 

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