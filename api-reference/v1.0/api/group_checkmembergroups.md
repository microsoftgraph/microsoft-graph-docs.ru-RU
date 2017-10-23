# <a name="group-checkmembergroups"></a><span data-ttu-id="84fe9-101">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="84fe9-101">group: checkMemberGroups</span></span>
<span data-ttu-id="84fe9-p101">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="84fe9-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span> 

<span data-ttu-id="84fe9-p102">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="84fe9-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="84fe9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84fe9-108">Permissions</span></span>
<span data-ttu-id="84fe9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="84fe9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="84fe9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84fe9-111">Permission type</span></span>      | <span data-ttu-id="84fe9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84fe9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84fe9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84fe9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="84fe9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84fe9-114">Not supported.</span></span>    |
|<span data-ttu-id="84fe9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84fe9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84fe9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84fe9-116">Not supported.</span></span>    |
|<span data-ttu-id="84fe9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84fe9-117">Application</span></span> | <span data-ttu-id="84fe9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84fe9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84fe9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84fe9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="84fe9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84fe9-120">Request headers</span></span>
| <span data-ttu-id="84fe9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="84fe9-121">Name</span></span>       | <span data-ttu-id="84fe9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="84fe9-122">Type</span></span> | <span data-ttu-id="84fe9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="84fe9-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84fe9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="84fe9-124">Authorization</span></span>  | <span data-ttu-id="84fe9-125">string</span><span class="sxs-lookup"><span data-stu-id="84fe9-125">string</span></span>  | <span data-ttu-id="84fe9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84fe9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84fe9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84fe9-128">Request body</span></span>
<span data-ttu-id="84fe9-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="84fe9-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="84fe9-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="84fe9-130">Parameter</span></span>    | <span data-ttu-id="84fe9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84fe9-131">Type</span></span>   |<span data-ttu-id="84fe9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84fe9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84fe9-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="84fe9-133">groupIds</span></span>|<span data-ttu-id="84fe9-134">String</span><span class="sxs-lookup"><span data-stu-id="84fe9-134">String</span></span>|<span data-ttu-id="84fe9-135">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="84fe9-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="84fe9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="84fe9-136">Response</span></span>

<span data-ttu-id="84fe9-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84fe9-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84fe9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="84fe9-138">Example</span></span>
<span data-ttu-id="84fe9-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="84fe9-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84fe9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="84fe9-140">Request</span></span>
<span data-ttu-id="84fe9-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84fe9-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="84fe9-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="84fe9-142">Response</span></span>
<span data-ttu-id="84fe9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84fe9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
