# <a name="group-checkmembergroups"></a><span data-ttu-id="a90bb-101">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a90bb-101">group: checkMemberGroups</span></span>

<span data-ttu-id="a90bb-p101">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="a90bb-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="a90bb-p102">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="a90bb-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="a90bb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a90bb-108">Permissions</span></span>

<span data-ttu-id="a90bb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a90bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a90bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a90bb-111">Permission type</span></span>                        | <span data-ttu-id="a90bb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a90bb-112">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a90bb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a90bb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a90bb-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a90bb-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a90bb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a90bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a90bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90bb-116">Not supported.</span></span>                                                                              |
| <span data-ttu-id="a90bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a90bb-117">Application</span></span>                            | <span data-ttu-id="a90bb-118">_Group.Read.All_, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="a90bb-118">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span> <span data-ttu-id="a90bb-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a90bb-119">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="a90bb-120">**Примечание:** в настоящее время для вызова этого API требуется разрешение `Directory.Read.All` или выше.</span><span class="sxs-lookup"><span data-stu-id="a90bb-120">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="a90bb-121">При использовании разрешения `Gorup.Read.All` будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="a90bb-121">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="a90bb-122">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="a90bb-122">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="a90bb-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a90bb-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="a90bb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a90bb-124">Request headers</span></span>

| <span data-ttu-id="a90bb-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a90bb-125">Name</span></span>          | <span data-ttu-id="a90bb-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a90bb-126">Type</span></span>   | <span data-ttu-id="a90bb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a90bb-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a90bb-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a90bb-128">Authorization</span></span> | <span data-ttu-id="a90bb-129">строка</span><span class="sxs-lookup"><span data-stu-id="a90bb-129">string</span></span> | <span data-ttu-id="a90bb-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a90bb-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a90bb-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a90bb-132">Request body</span></span>

<span data-ttu-id="a90bb-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a90bb-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a90bb-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="a90bb-134">Parameter</span></span> | <span data-ttu-id="a90bb-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a90bb-135">Type</span></span>              | <span data-ttu-id="a90bb-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a90bb-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="a90bb-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="a90bb-137">groupIds</span></span>  | <span data-ttu-id="a90bb-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a90bb-138">String collection</span></span> | <span data-ttu-id="a90bb-139">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="a90bb-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="a90bb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a90bb-140">Response</span></span>

<span data-ttu-id="a90bb-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a90bb-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a90bb-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a90bb-142">Example</span></span>

<span data-ttu-id="a90bb-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a90bb-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a90bb-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a90bb-144">Request</span></span>

<span data-ttu-id="a90bb-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a90bb-145">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a90bb-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90bb-146">Response</span></span>

<span data-ttu-id="a90bb-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a90bb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
