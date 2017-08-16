# <a name="add-group-owner"></a><span data-ttu-id="07581-101">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="07581-101">Add group owner</span></span>
<span data-ttu-id="07581-p101">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="07581-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07581-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="07581-104">Prerequisites</span></span>
<span data-ttu-id="07581-105">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="07581-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="07581-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07581-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="07581-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07581-107">Request headers</span></span>
| <span data-ttu-id="07581-108">Имя</span><span class="sxs-lookup"><span data-stu-id="07581-108">Name</span></span>       | <span data-ttu-id="07581-109">Тип</span><span class="sxs-lookup"><span data-stu-id="07581-109">Type</span></span> | <span data-ttu-id="07581-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07581-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07581-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="07581-111">Authorization</span></span>  | <span data-ttu-id="07581-112">string</span><span class="sxs-lookup"><span data-stu-id="07581-112">string</span></span>  | <span data-ttu-id="07581-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07581-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07581-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07581-115">Request body</span></span>
<span data-ttu-id="07581-116">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07581-116">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="07581-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="07581-117">Response</span></span>

<span data-ttu-id="07581-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="07581-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07581-120">Пример</span><span class="sxs-lookup"><span data-stu-id="07581-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07581-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="07581-121">Request</span></span>
<span data-ttu-id="07581-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07581-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="07581-123">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07581-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="07581-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="07581-124">Response</span></span>
<span data-ttu-id="07581-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07581-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
