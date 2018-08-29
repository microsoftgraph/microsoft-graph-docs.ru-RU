# <a name="get-deleted-item"></a><span data-ttu-id="053f7-101">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="053f7-101">Get deleted item</span></span>

<span data-ttu-id="053f7-102">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="053f7-102">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="053f7-103">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="053f7-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="053f7-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="053f7-104">Permissions</span></span>
<span data-ttu-id="053f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="053f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="053f7-107">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="053f7-107">For users:</span></span>

|<span data-ttu-id="053f7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="053f7-108">Permission type</span></span>      | <span data-ttu-id="053f7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="053f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="053f7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="053f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="053f7-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="053f7-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="053f7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="053f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="053f7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="053f7-113">Not supported.</span></span> |
|<span data-ttu-id="053f7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="053f7-114">Application</span></span> | <span data-ttu-id="053f7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053f7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="053f7-116">Для групп:</span><span class="sxs-lookup"><span data-stu-id="053f7-116">For groups:</span></span>

|<span data-ttu-id="053f7-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="053f7-117">Permission type</span></span>      | <span data-ttu-id="053f7-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="053f7-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="053f7-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="053f7-119">Delegated (work or school account)</span></span> | <span data-ttu-id="053f7-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="053f7-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="053f7-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="053f7-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="053f7-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="053f7-122">Not supported.</span></span>    |
|<span data-ttu-id="053f7-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="053f7-123">Application</span></span> | <span data-ttu-id="053f7-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053f7-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="053f7-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="053f7-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="053f7-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="053f7-126">Optional query parameters</span></span>
<span data-ttu-id="053f7-127">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="053f7-127">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="053f7-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="053f7-128">Request headers</span></span>
| <span data-ttu-id="053f7-129">Имя</span><span class="sxs-lookup"><span data-stu-id="053f7-129">Name</span></span>      |<span data-ttu-id="053f7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="053f7-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="053f7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="053f7-131">Authorization</span></span>  | <span data-ttu-id="053f7-132">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="053f7-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="053f7-133">Accept</span><span class="sxs-lookup"><span data-stu-id="053f7-133">Accept</span></span>  | <span data-ttu-id="053f7-134">application/json</span><span class="sxs-lookup"><span data-stu-id="053f7-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="053f7-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="053f7-135">Request body</span></span>
<span data-ttu-id="053f7-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="053f7-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="053f7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="053f7-137">Response</span></span>

<span data-ttu-id="053f7-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="053f7-138">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="053f7-139">Пример</span><span class="sxs-lookup"><span data-stu-id="053f7-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="053f7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="053f7-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="053f7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="053f7-141">Response</span></span>
<span data-ttu-id="053f7-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="053f7-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->