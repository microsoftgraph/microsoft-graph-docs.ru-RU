# <a name="check-member-groups"></a><span data-ttu-id="e9813-101">Проверка групп элементов</span><span class="sxs-lookup"><span data-stu-id="e9813-101">Check member groups</span></span>

<span data-ttu-id="e9813-p101">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="e9813-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9813-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9813-104">Permissions</span></span>
<span data-ttu-id="e9813-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9813-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9813-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9813-107">Permission type</span></span>      | <span data-ttu-id="e9813-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9813-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9813-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9813-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e9813-110">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9813-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="e9813-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9813-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9813-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9813-112">Not supported.</span></span>    |
|<span data-ttu-id="e9813-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9813-113">Application</span></span> | <span data-ttu-id="e9813-114">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9813-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9813-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9813-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="e9813-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9813-116">Request headers</span></span>
| <span data-ttu-id="e9813-117">Имя</span><span class="sxs-lookup"><span data-stu-id="e9813-117">Name</span></span>       | <span data-ttu-id="e9813-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e9813-118">Type</span></span> | <span data-ttu-id="e9813-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e9813-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9813-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9813-120">Authorization</span></span>  | <span data-ttu-id="e9813-121">строка</span><span class="sxs-lookup"><span data-stu-id="e9813-121">string</span></span>  | <span data-ttu-id="e9813-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9813-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9813-124">Тип содеримого</span><span class="sxs-lookup"><span data-stu-id="e9813-124">Content-Type</span></span>  | <span data-ttu-id="e9813-125">строка</span><span class="sxs-lookup"><span data-stu-id="e9813-125">string</span></span> | <span data-ttu-id="e9813-126">приложение/json</span><span class="sxs-lookup"><span data-stu-id="e9813-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9813-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9813-127">Request body</span></span>
<span data-ttu-id="e9813-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e9813-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9813-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e9813-129">Parameter</span></span>    | <span data-ttu-id="e9813-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e9813-130">Type</span></span>   |<span data-ttu-id="e9813-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9813-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9813-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="e9813-132">groupIds</span></span>|<span data-ttu-id="e9813-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9813-133">String collection</span></span>|<span data-ttu-id="e9813-p104">Коллекция, содержащая идентификатор объектов групп, в которых нужно проверить членство. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="e9813-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="e9813-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9813-136">Response</span></span>

<span data-ttu-id="e9813-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9813-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9813-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e9813-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e9813-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9813-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="e9813-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9813-140">Response</span></span>
<span data-ttu-id="e9813-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9813-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
