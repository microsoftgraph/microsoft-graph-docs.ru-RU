# <a name="assign-a-manager"></a><span data-ttu-id="32ded-101">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="32ded-101">Assign a manager</span></span>

<span data-ttu-id="32ded-102">С помощью этого API можно назначить руководителя пользователю.</span><span class="sxs-lookup"><span data-stu-id="32ded-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="32ded-103">Примечание. Назначать подчиненных невозможно. Вместо этого используйте данный API.</span><span class="sxs-lookup"><span data-stu-id="32ded-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32ded-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32ded-104">Prerequisites</span></span>
<span data-ttu-id="32ded-105">Для применения этого API требуется одна из указанных ниже **областей**. *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="32ded-105">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="32ded-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32ded-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="32ded-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32ded-107">Request headers</span></span>
| <span data-ttu-id="32ded-108">Имя</span><span class="sxs-lookup"><span data-stu-id="32ded-108">Name</span></span>       | <span data-ttu-id="32ded-109">Тип</span><span class="sxs-lookup"><span data-stu-id="32ded-109">Type</span></span> | <span data-ttu-id="32ded-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32ded-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="32ded-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="32ded-111">Authorization</span></span>  | <span data-ttu-id="32ded-112">string</span><span class="sxs-lookup"><span data-stu-id="32ded-112">string</span></span>  | <span data-ttu-id="32ded-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32ded-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32ded-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32ded-115">Request body</span></span>
<span data-ttu-id="32ded-116">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32ded-116">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="32ded-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="32ded-117">Response</span></span>

<span data-ttu-id="32ded-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="32ded-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32ded-120">Пример</span><span class="sxs-lookup"><span data-stu-id="32ded-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32ded-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="32ded-121">Request</span></span>
<span data-ttu-id="32ded-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32ded-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="32ded-123">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32ded-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="32ded-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="32ded-124">Response</span></span>
<span data-ttu-id="32ded-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="32ded-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
