# <a name="user-getmemberobjects"></a><span data-ttu-id="69a10-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="69a10-101">user: getMemberObjects</span></span>
<span data-ttu-id="69a10-p101">Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="69a10-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="69a10-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69a10-104">Permissions</span></span>
<span data-ttu-id="69a10-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69a10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="69a10-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69a10-107">Permission type</span></span>      | <span data-ttu-id="69a10-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69a10-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69a10-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69a10-109">Delegated (work or school account)</span></span> | <span data-ttu-id="69a10-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69a10-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="69a10-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69a10-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69a10-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69a10-112">Not supported.</span></span>    |
|<span data-ttu-id="69a10-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69a10-113">Application</span></span> | <span data-ttu-id="69a10-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69a10-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69a10-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69a10-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="69a10-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69a10-116">Request headers</span></span>
| <span data-ttu-id="69a10-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69a10-117">Header</span></span>       | <span data-ttu-id="69a10-118">Значение</span><span class="sxs-lookup"><span data-stu-id="69a10-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69a10-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69a10-119">Authorization</span></span>  | <span data-ttu-id="69a10-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69a10-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="69a10-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69a10-122">Content-Type</span></span>  | <span data-ttu-id="69a10-123">application/json</span><span class="sxs-lookup"><span data-stu-id="69a10-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69a10-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69a10-124">Request body</span></span>
<span data-ttu-id="69a10-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="69a10-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69a10-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="69a10-126">Parameter</span></span>    | <span data-ttu-id="69a10-127">Тип</span><span class="sxs-lookup"><span data-stu-id="69a10-127">Type</span></span>   |<span data-ttu-id="69a10-128">Описание</span><span class="sxs-lookup"><span data-stu-id="69a10-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69a10-129">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="69a10-129">securityEnabledOnly</span></span>|<span data-ttu-id="69a10-130">Логическое</span><span class="sxs-lookup"><span data-stu-id="69a10-130">Boolean</span></span>|<span data-ttu-id="69a10-p104">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является пользователь. Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="69a10-p104">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="69a10-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="69a10-133">Response</span></span>

<span data-ttu-id="69a10-134">В случае успеха этот метод возвращает код отклика `200, OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="69a10-134">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="69a10-135">Пример</span><span class="sxs-lookup"><span data-stu-id="69a10-135">Example</span></span>
<span data-ttu-id="69a10-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="69a10-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="69a10-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="69a10-137">Request</span></span>
<span data-ttu-id="69a10-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69a10-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="69a10-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="69a10-139">Response</span></span>
<span data-ttu-id="69a10-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="69a10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
