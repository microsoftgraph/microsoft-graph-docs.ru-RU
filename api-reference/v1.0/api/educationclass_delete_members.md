# <a name="remove-a-student"></a><span data-ttu-id="757f7-101">Удаление учащегося</span><span class="sxs-lookup"><span data-stu-id="757f7-101">Remove a student</span></span>

<span data-ttu-id="757f7-102">Удаляет [educationUser](../resources/educationuser.md) из [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="757f7-102">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="757f7-103">**Примечание.** Преподаватели _и_ учащиеся включены в коллекцию **members** курса.</span><span class="sxs-lookup"><span data-stu-id="757f7-103">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="757f7-104">Перед вызовом этого API нужно проверить, не представляет ли удаляемый объект **educationUser** преподавателя.</span><span class="sxs-lookup"><span data-stu-id="757f7-104">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="757f7-105">Для этого необходимо получить список преподавателей путем вызова [educationclass_list_teachers](educationclass_list_teachers.md) и проверить, не возвращается ли в этом списке ИД удаляемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="757f7-105">Get the list of teachers by calling [educationclass_list_teachers](educationclass_list_teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="757f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="757f7-106">Permissions</span></span>
<span data-ttu-id="757f7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="757f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="757f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="757f7-109">Permission type</span></span>      | <span data-ttu-id="757f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="757f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="757f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="757f7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="757f7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="757f7-112">Not supported.</span></span>  |
|<span data-ttu-id="757f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="757f7-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="757f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="757f7-114">Not supported.</span></span>  |
|<span data-ttu-id="757f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="757f7-115">Application</span></span> | <span data-ttu-id="757f7-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="757f7-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="757f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="757f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="757f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="757f7-118">Request headers</span></span>
| <span data-ttu-id="757f7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="757f7-119">Header</span></span>       | <span data-ttu-id="757f7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="757f7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="757f7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="757f7-121">Authorization</span></span>  | <span data-ttu-id="757f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="757f7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="757f7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="757f7-124">Request body</span></span>
<span data-ttu-id="757f7-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="757f7-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="757f7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="757f7-126">Response</span></span>
<span data-ttu-id="757f7-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="757f7-127">If successful, this method returns a `204 No Content` response code and an event object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="757f7-128">Пример</span><span class="sxs-lookup"><span data-stu-id="757f7-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="757f7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="757f7-129">Request</span></span>
<span data-ttu-id="757f7-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="757f7-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="757f7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="757f7-131">Response</span></span>
<span data-ttu-id="757f7-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="757f7-132">The following is an example of the response.</span></span> 
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
