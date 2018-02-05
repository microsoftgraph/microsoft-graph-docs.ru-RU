# <a name="checkmembergroups"></a><span data-ttu-id="d1716-101">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d1716-101">checkMemberGroups</span></span>
<span data-ttu-id="d1716-p101">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="d1716-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span> 

<span data-ttu-id="d1716-p102">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="d1716-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d1716-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1716-108">Permissions</span></span>
<span data-ttu-id="d1716-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d1716-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="d1716-111">**Примечание.** В настоящее время для работы с этим API требуется разрешение Directory.Read.All или выше.</span><span class="sxs-lookup"><span data-stu-id="d1716-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="d1716-112">При использовании разрешения User.Read.All или User.ReadWrite.All возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="d1716-112">Using the User.Read.All or User.ReadWrite.All permissions will return an error.</span></span> <span data-ttu-id="d1716-113">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="d1716-113">This is a known bug.</span></span>

|<span data-ttu-id="d1716-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1716-114">Permission type</span></span>      | <span data-ttu-id="d1716-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1716-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1716-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1716-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d1716-117">*User.Read.All*, *User.ReadWrite.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1716-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1716-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1716-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1716-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1716-119">Not supported.</span></span>    |
|<span data-ttu-id="d1716-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d1716-120">Application</span></span> | <span data-ttu-id="d1716-121">*User.Read.All*, *User.ReadWrite.All*, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1716-121">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1716-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1716-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="d1716-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1716-123">Request headers</span></span>
| <span data-ttu-id="d1716-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1716-124">Header</span></span>       | <span data-ttu-id="d1716-125">Значение</span><span class="sxs-lookup"><span data-stu-id="d1716-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1716-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1716-126">Authorization</span></span>  | <span data-ttu-id="d1716-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1716-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d1716-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1716-129">Content-Type</span></span>  | <span data-ttu-id="d1716-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d1716-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1716-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1716-131">Request body</span></span>
<span data-ttu-id="d1716-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d1716-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1716-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="d1716-133">Parameter</span></span>    | <span data-ttu-id="d1716-134">Тип</span><span class="sxs-lookup"><span data-stu-id="d1716-134">Type</span></span>   |<span data-ttu-id="d1716-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d1716-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1716-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="d1716-136">groupIds</span></span>|<span data-ttu-id="d1716-137">String</span><span class="sxs-lookup"><span data-stu-id="d1716-137">String</span></span>|<span data-ttu-id="d1716-138">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="d1716-138">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="d1716-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1716-139">Response</span></span>

<span data-ttu-id="d1716-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1716-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1716-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d1716-141">Example</span></span>
<span data-ttu-id="d1716-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1716-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1716-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1716-143">Request</span></span>
<span data-ttu-id="d1716-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1716-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="d1716-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1716-145">Response</span></span>
<span data-ttu-id="d1716-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d1716-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
