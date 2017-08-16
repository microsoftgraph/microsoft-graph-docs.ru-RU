# <a name="add-member"></a><span data-ttu-id="7a76c-101">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="7a76c-101">Add member</span></span>

<span data-ttu-id="7a76c-p101">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**. Вы можете добавлять пользователей или другие группы. Важно! В группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="7a76c-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a76c-105">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7a76c-105">Prerequisites</span></span>
<span data-ttu-id="7a76c-106">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="7a76c-106">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="7a76c-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a76c-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7a76c-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a76c-108">Request headers</span></span>
| <span data-ttu-id="7a76c-109">Имя</span><span class="sxs-lookup"><span data-stu-id="7a76c-109">Name</span></span>       | <span data-ttu-id="7a76c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7a76c-110">Type</span></span> | <span data-ttu-id="7a76c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7a76c-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7a76c-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a76c-112">Authorization</span></span>  | <span data-ttu-id="7a76c-113">string</span><span class="sxs-lookup"><span data-stu-id="7a76c-113">string</span></span>  | <span data-ttu-id="7a76c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a76c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a76c-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a76c-116">Request body</span></span>
<span data-ttu-id="7a76c-117">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a76c-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="7a76c-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a76c-118">Response</span></span>

<span data-ttu-id="7a76c-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7a76c-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a76c-121">Пример</span><span class="sxs-lookup"><span data-stu-id="7a76c-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a76c-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a76c-122">Request</span></span>
<span data-ttu-id="7a76c-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a76c-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="7a76c-124">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a76c-124">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="7a76c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a76c-125">Response</span></span>
<span data-ttu-id="7a76c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7a76c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->