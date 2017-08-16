# <a name="activate-directoryrole"></a><span data-ttu-id="9e0d0-101">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="9e0d0-101">Activate directoryRole</span></span>

<span data-ttu-id="9e0d0-p101">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="9e0d0-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e0d0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9e0d0-106">Prerequisites</span></span>
<span data-ttu-id="9e0d0-107">Для применения этого API требуется одна из указанных ниже **областей**. *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="9e0d0-107">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="9e0d0-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e0d0-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="9e0d0-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e0d0-109">Request headers</span></span>
| <span data-ttu-id="9e0d0-110">Имя</span><span class="sxs-lookup"><span data-stu-id="9e0d0-110">Name</span></span>       | <span data-ttu-id="9e0d0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9e0d0-111">Type</span></span> | <span data-ttu-id="9e0d0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9e0d0-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e0d0-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e0d0-113">Authorization</span></span>  | <span data-ttu-id="9e0d0-114">string</span><span class="sxs-lookup"><span data-stu-id="9e0d0-114">string</span></span>  | <span data-ttu-id="9e0d0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e0d0-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e0d0-117">Content-Type</span></span>  | <span data-ttu-id="9e0d0-118">application/json</span><span class="sxs-lookup"><span data-stu-id="9e0d0-118">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e0d0-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e0d0-119">Request body</span></span>
<span data-ttu-id="9e0d0-120">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-120">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="9e0d0-121">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-121">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="9e0d0-122">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="9e0d0-122">Required parameter</span></span> | <span data-ttu-id="9e0d0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9e0d0-123">Type</span></span> | <span data-ttu-id="9e0d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9e0d0-124">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="9e0d0-125">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9e0d0-125">roleTemplateId</span></span> | <span data-ttu-id="9e0d0-126">string</span><span class="sxs-lookup"><span data-stu-id="9e0d0-126">string</span></span> | <span data-ttu-id="9e0d0-p103">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-p103">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="9e0d0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e0d0-129">Response</span></span>

<span data-ttu-id="9e0d0-130">В случае успеха этот метод возвратит код отклика `201, Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-130">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e0d0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e0d0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e0d0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e0d0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="9e0d0-133">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9e0d0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e0d0-134">Response</span></span>
<span data-ttu-id="9e0d0-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e0d0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
