# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="100f5-101">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="100f5-101">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="100f5-102">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="100f5-102">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="100f5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="100f5-103">Permissions</span></span>

<span data-ttu-id="100f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="100f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="100f5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="100f5-106">Permission type</span></span>      | <span data-ttu-id="100f5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="100f5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="100f5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="100f5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="100f5-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="100f5-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="100f5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="100f5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="100f5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="100f5-111">Not supported.</span></span>    |
|<span data-ttu-id="100f5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="100f5-112">Application</span></span> | <span data-ttu-id="100f5-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="100f5-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="100f5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="100f5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="100f5-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="100f5-115">Request headers</span></span>

| <span data-ttu-id="100f5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="100f5-116">Name</span></span> | <span data-ttu-id="100f5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="100f5-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="100f5-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="100f5-118">Authorization</span></span> | <span data-ttu-id="100f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="100f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="100f5-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="100f5-121">Content-Type</span></span>  | <span data-ttu-id="100f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="100f5-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="100f5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="100f5-123">Request body</span></span>
<span data-ttu-id="100f5-124">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="100f5-124">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="100f5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="100f5-125">Response</span></span>

<span data-ttu-id="100f5-126">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="100f5-126">If successful, this method returns a `201 Created` response code and [profilePhoto](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="100f5-127">Пример</span><span class="sxs-lookup"><span data-stu-id="100f5-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="100f5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="100f5-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="100f5-129">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="100f5-129">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="100f5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="100f5-130">Response</span></span>

<span data-ttu-id="100f5-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="100f5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->