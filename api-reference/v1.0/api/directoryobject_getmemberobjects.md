# <a name="get-member-objects"></a><span data-ttu-id="6a6c1-101">Вывод объектов элементов</span><span class="sxs-lookup"><span data-stu-id="6a6c1-101">Get member objects</span></span>

 <span data-ttu-id="6a6c1-p101">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-p101">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="6a6c1-104">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-104">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a6c1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a6c1-105">Permissions</span></span>
<span data-ttu-id="6a6c1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a6c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a6c1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a6c1-108">Permission type</span></span>      | <span data-ttu-id="6a6c1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a6c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a6c1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a6c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a6c1-111">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a6c1-111">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="6a6c1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a6c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a6c1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-113">Not supported.</span></span>    |
|<span data-ttu-id="6a6c1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a6c1-114">Application</span></span> | <span data-ttu-id="6a6c1-115">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a6c1-115">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a6c1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a6c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="6a6c1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a6c1-117">Request headers</span></span>
| <span data-ttu-id="6a6c1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6a6c1-118">Name</span></span>       | <span data-ttu-id="6a6c1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6c1-119">Type</span></span> | <span data-ttu-id="6a6c1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6c1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6a6c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a6c1-121">Authorization</span></span>  | <span data-ttu-id="6a6c1-122">string</span><span class="sxs-lookup"><span data-stu-id="6a6c1-122">string</span></span>  | <span data-ttu-id="6a6c1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a6c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a6c1-125">Content-Type</span></span>  | <span data-ttu-id="6a6c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a6c1-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a6c1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a6c1-127">Request body</span></span>
<span data-ttu-id="6a6c1-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6a6c1-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="6a6c1-129">Parameter</span></span>    | <span data-ttu-id="6a6c1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6c1-130">Type</span></span>   |<span data-ttu-id="6a6c1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6c1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a6c1-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6a6c1-132">securityEnabledOnly</span></span>|<span data-ttu-id="6a6c1-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="6a6c1-133">Boolean</span></span>| <span data-ttu-id="6a6c1-p104">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="6a6c1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a6c1-136">Response</span></span>

<span data-ttu-id="6a6c1-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a6c1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6a6c1-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6a6c1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a6c1-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="6a6c1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a6c1-140">Response</span></span>
<span data-ttu-id="6a6c1-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a6c1-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
