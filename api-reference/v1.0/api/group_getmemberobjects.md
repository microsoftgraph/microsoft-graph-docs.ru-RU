# <a name="group-getmemberobjects"></a><span data-ttu-id="e7515-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e7515-101">group: getMemberObjects</span></span>
<span data-ttu-id="e7515-p101">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="e7515-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7515-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7515-105">Permissions</span></span>
<span data-ttu-id="e7515-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7515-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7515-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7515-108">Permission type</span></span>      | <span data-ttu-id="e7515-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7515-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7515-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7515-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7515-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7515-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e7515-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7515-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7515-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7515-113">Not supported.</span></span>    |
|<span data-ttu-id="e7515-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7515-114">Application</span></span> | <span data-ttu-id="e7515-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7515-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7515-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7515-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="e7515-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7515-117">Request headers</span></span>
| <span data-ttu-id="e7515-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e7515-118">Name</span></span>       | <span data-ttu-id="e7515-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e7515-119">Type</span></span> | <span data-ttu-id="e7515-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e7515-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7515-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7515-121">Authorization</span></span>  | <span data-ttu-id="e7515-122">string</span><span class="sxs-lookup"><span data-stu-id="e7515-122">string</span></span>  | <span data-ttu-id="e7515-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7515-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7515-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7515-125">Request body</span></span>
<span data-ttu-id="e7515-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e7515-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7515-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="e7515-127">Parameter</span></span>    | <span data-ttu-id="e7515-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e7515-128">Type</span></span>   |<span data-ttu-id="e7515-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e7515-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7515-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e7515-130">securityEnabledOnly</span></span>|<span data-ttu-id="e7515-131">Логическое</span><span class="sxs-lookup"><span data-stu-id="e7515-131">Boolean</span></span>| <span data-ttu-id="e7515-p104">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="e7515-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="e7515-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7515-134">Response</span></span>
<span data-ttu-id="e7515-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="e7515-135">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="e7515-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e7515-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e7515-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7515-137">Request</span></span>
<span data-ttu-id="e7515-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7515-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="e7515-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7515-139">Response</span></span>
<span data-ttu-id="e7515-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7515-140">The following is an example of the response.</span></span>
><span data-ttu-id="e7515-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e7515-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7515-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7515-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
