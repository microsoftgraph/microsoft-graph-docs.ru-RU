# <a name="remove-a-student"></a><span data-ttu-id="9a226-101">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="9a226-101">Remove a student</span></span>

<span data-ttu-id="9a226-102">Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="9a226-102">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="9a226-103">**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса.</span><span class="sxs-lookup"><span data-stu-id="9a226-103">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="9a226-104">Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.</span><span class="sxs-lookup"><span data-stu-id="9a226-104">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="9a226-105">Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass_list_teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a226-105">Get the list of teachers by calling [educationclass_list_teachers](educationclass_list_teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a226-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a226-106">Permissions</span></span>
<span data-ttu-id="9a226-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a226-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a226-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a226-109">Permission type</span></span>      | <span data-ttu-id="9a226-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a226-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a226-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a226-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9a226-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a226-112">Not supported.</span></span>  |
|<span data-ttu-id="9a226-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a226-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9a226-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a226-114">Not supported.</span></span>  |
|<span data-ttu-id="9a226-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a226-115">Application</span></span> | <span data-ttu-id="9a226-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a226-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9a226-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a226-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9a226-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a226-118">Request headers</span></span>
| <span data-ttu-id="9a226-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a226-119">Header</span></span>       | <span data-ttu-id="9a226-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9a226-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a226-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a226-121">Authorization</span></span>  | <span data-ttu-id="9a226-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a226-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a226-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a226-124">Request body</span></span>
<span data-ttu-id="9a226-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a226-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9a226-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a226-126">Response</span></span>
<span data-ttu-id="9a226-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="9a226-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a226-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9a226-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a226-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a226-129">Request</span></span>
<span data-ttu-id="9a226-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a226-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```

##### <a name="response"></a><span data-ttu-id="9a226-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a226-131">Response</span></span>
<span data-ttu-id="9a226-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9a226-132">The following is an example of the response.</span></span> 
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
