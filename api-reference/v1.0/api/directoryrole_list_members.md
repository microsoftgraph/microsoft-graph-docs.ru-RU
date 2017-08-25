# <a name="list-members"></a><span data-ttu-id="739fa-101">Список участников</span><span class="sxs-lookup"><span data-stu-id="739fa-101">List members</span></span>

<span data-ttu-id="739fa-p101">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="739fa-p101">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="739fa-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="739fa-104">Permissions</span></span>
<span data-ttu-id="739fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="739fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="739fa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="739fa-107">Permission type</span></span>      | <span data-ttu-id="739fa-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="739fa-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="739fa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="739fa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="739fa-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="739fa-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="739fa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="739fa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="739fa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="739fa-112">Not supported.</span></span>    | 
|<span data-ttu-id="739fa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="739fa-113">Application</span></span> | <span data-ttu-id="739fa-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="739fa-114">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="739fa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="739fa-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="739fa-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="739fa-116">Optional query parameters</span></span>
<span data-ttu-id="739fa-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="739fa-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="739fa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="739fa-118">Request headers</span></span>
| <span data-ttu-id="739fa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="739fa-119">Name</span></span>       | <span data-ttu-id="739fa-120">Тип</span><span class="sxs-lookup"><span data-stu-id="739fa-120">Type</span></span> | <span data-ttu-id="739fa-121">Описание</span><span class="sxs-lookup"><span data-stu-id="739fa-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="739fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="739fa-122">Authorization</span></span>  | <span data-ttu-id="739fa-123">string</span><span class="sxs-lookup"><span data-stu-id="739fa-123">string</span></span>  | <span data-ttu-id="739fa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="739fa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="739fa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="739fa-126">Request body</span></span>
<span data-ttu-id="739fa-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="739fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="739fa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="739fa-128">Response</span></span>

<span data-ttu-id="739fa-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="739fa-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="739fa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="739fa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="739fa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="739fa-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="739fa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="739fa-132">Response</span></span>
<span data-ttu-id="739fa-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="739fa-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->