# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="4db0d-101">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="4db0d-101">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="4db0d-102">Добавляет группу к политике жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="4db0d-102">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="4db0d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4db0d-103">Permissions</span></span>

<span data-ttu-id="4db0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4db0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4db0d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4db0d-106">Permission type</span></span>      | <span data-ttu-id="4db0d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4db0d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4db0d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4db0d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4db0d-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db0d-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4db0d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4db0d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4db0d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4db0d-111">Not supported.</span></span>    |
|<span data-ttu-id="4db0d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4db0d-112">Application</span></span> | <span data-ttu-id="4db0d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db0d-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4db0d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4db0d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="4db0d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4db0d-115">Request headers</span></span>

| <span data-ttu-id="4db0d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4db0d-116">Name</span></span> | <span data-ttu-id="4db0d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4db0d-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4db0d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4db0d-118">Authorization</span></span> | <span data-ttu-id="4db0d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4db0d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4db0d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4db0d-121">Content-Type</span></span>  | <span data-ttu-id="4db0d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4db0d-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4db0d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4db0d-123">Request body</span></span>
<span data-ttu-id="4db0d-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4db0d-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4db0d-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4db0d-125">Parameter</span></span> | <span data-ttu-id="4db0d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4db0d-126">Type</span></span> | <span data-ttu-id="4db0d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4db0d-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4db0d-128">groupId</span><span class="sxs-lookup"><span data-stu-id="4db0d-128">groupId</span></span>|<span data-ttu-id="4db0d-129">GUID</span><span class="sxs-lookup"><span data-stu-id="4db0d-129">Guid</span></span>| <span data-ttu-id="4db0d-130">Идентификатор группы, которую нужно добавить к политике.</span><span class="sxs-lookup"><span data-stu-id="4db0d-130">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="4db0d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4db0d-131">Response</span></span>

<span data-ttu-id="4db0d-132">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4db0d-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="4db0d-133">Если к политике добавляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="4db0d-133">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="4db0d-134">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="4db0d-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="4db0d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4db0d-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4db0d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4db0d-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="4db0d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4db0d-137">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->