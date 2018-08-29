# <a name="get-member-groups"></a><span data-ttu-id="49f11-101">Вывод групп элементов</span><span class="sxs-lookup"><span data-stu-id="49f11-101">Get member groups</span></span>

<span data-ttu-id="49f11-p101">Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="49f11-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="49f11-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49f11-104">Permissions</span></span>
<span data-ttu-id="49f11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="49f11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="49f11-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49f11-107">Permission type</span></span>      | <span data-ttu-id="49f11-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49f11-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49f11-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49f11-109">Delegated (work or school account)</span></span> | <span data-ttu-id="49f11-110">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="49f11-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="49f11-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49f11-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49f11-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f11-112">Not supported.</span></span>    |
|<span data-ttu-id="49f11-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49f11-113">Application</span></span> | <span data-ttu-id="49f11-114">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="49f11-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49f11-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49f11-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="49f11-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49f11-116">Request headers</span></span>
| <span data-ttu-id="49f11-117">Имя</span><span class="sxs-lookup"><span data-stu-id="49f11-117">Name</span></span>       | <span data-ttu-id="49f11-118">Тип</span><span class="sxs-lookup"><span data-stu-id="49f11-118">Type</span></span> | <span data-ttu-id="49f11-119">Описание</span><span class="sxs-lookup"><span data-stu-id="49f11-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49f11-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49f11-120">Authorization</span></span>  | <span data-ttu-id="49f11-121">строка</span><span class="sxs-lookup"><span data-stu-id="49f11-121">string</span></span>  | <span data-ttu-id="49f11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49f11-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49f11-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49f11-124">Content-Type</span></span>   | <span data-ttu-id="49f11-125">строка</span><span class="sxs-lookup"><span data-stu-id="49f11-125">string</span></span>  | <span data-ttu-id="49f11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49f11-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49f11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49f11-127">Request body</span></span>
<span data-ttu-id="49f11-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="49f11-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49f11-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="49f11-129">Parameter</span></span>    | <span data-ttu-id="49f11-130">Тип</span><span class="sxs-lookup"><span data-stu-id="49f11-130">Type</span></span>   |<span data-ttu-id="49f11-131">Описание</span><span class="sxs-lookup"><span data-stu-id="49f11-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49f11-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="49f11-132">securityEnabledOnly</span></span>|<span data-ttu-id="49f11-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="49f11-133">Boolean</span></span>| <span data-ttu-id="49f11-p104">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="49f11-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="49f11-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f11-136">Response</span></span>

<span data-ttu-id="49f11-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49f11-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f11-138">Пример</span><span class="sxs-lookup"><span data-stu-id="49f11-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="49f11-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="49f11-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="49f11-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f11-140">Response</span></span>
<span data-ttu-id="49f11-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49f11-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
