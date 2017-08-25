# <a name="assign-a-manager"></a><span data-ttu-id="a718c-101">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="a718c-101">Assign a manager</span></span>

<span data-ttu-id="a718c-102">С помощью этого API можно назначить руководителя пользователю.</span><span class="sxs-lookup"><span data-stu-id="a718c-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="a718c-103">Примечание. Назначать подчиненных невозможно. Вместо этого используйте данный API.</span><span class="sxs-lookup"><span data-stu-id="a718c-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="a718c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a718c-104">Permissions</span></span>
<span data-ttu-id="a718c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a718c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a718c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a718c-107">Permission type</span></span>      | <span data-ttu-id="a718c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a718c-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a718c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a718c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a718c-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a718c-110">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="a718c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a718c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a718c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a718c-112">Not supported.</span></span>    | 
|<span data-ttu-id="a718c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a718c-113">Application</span></span> | <span data-ttu-id="a718c-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a718c-114">Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a718c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a718c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a718c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a718c-116">Request headers</span></span>
| <span data-ttu-id="a718c-117">Имя</span><span class="sxs-lookup"><span data-stu-id="a718c-117">Name</span></span>       | <span data-ttu-id="a718c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="a718c-118">Type</span></span> | <span data-ttu-id="a718c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a718c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a718c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a718c-120">Authorization</span></span>  | <span data-ttu-id="a718c-121">string</span><span class="sxs-lookup"><span data-stu-id="a718c-121">string</span></span>  | <span data-ttu-id="a718c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a718c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a718c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a718c-124">Request body</span></span>
<span data-ttu-id="a718c-125">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a718c-125">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a718c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a718c-126">Response</span></span>

<span data-ttu-id="a718c-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a718c-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a718c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a718c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a718c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a718c-130">Request</span></span>
<span data-ttu-id="a718c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a718c-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="a718c-132">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a718c-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="a718c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a718c-133">Response</span></span>
<span data-ttu-id="a718c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a718c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
