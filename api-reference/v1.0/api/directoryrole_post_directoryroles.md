# <a name="activate-directoryrole"></a><span data-ttu-id="ba8b4-101">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="ba8b4-101">Activate directoryRole</span></span>

<span data-ttu-id="ba8b4-p101">Активация роли каталога. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируются только неявные роли каталога пользователей, а также роли каталога администраторов организации. Чтобы получить доступ к членам и назначить для них другую роль каталога, сначала следует активировать ее с помощью соответствующего шаблона роли каталога ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="ba8b4-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba8b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8b4-106">Permissions</span></span>
<span data-ttu-id="ba8b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba8b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba8b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8b4-109">Permission type</span></span>      | <span data-ttu-id="ba8b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba8b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba8b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba8b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ba8b4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba8b4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba8b4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba8b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba8b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-114">Not supported.</span></span>    |
|<span data-ttu-id="ba8b4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba8b4-115">Application</span></span> | <span data-ttu-id="ba8b4-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8b4-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba8b4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba8b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="ba8b4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba8b4-118">Request headers</span></span>
| <span data-ttu-id="ba8b4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba8b4-119">Name</span></span>       | <span data-ttu-id="ba8b4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ba8b4-120">Type</span></span> | <span data-ttu-id="ba8b4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ba8b4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba8b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8b4-122">Authorization</span></span>  | <span data-ttu-id="ba8b4-123">string</span><span class="sxs-lookup"><span data-stu-id="ba8b4-123">string</span></span>  | <span data-ttu-id="ba8b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba8b4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba8b4-126">Content-Type</span></span>  | <span data-ttu-id="ba8b4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ba8b4-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba8b4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba8b4-128">Request body</span></span>
<span data-ttu-id="ba8b4-129">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-129">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="ba8b4-130">В приведенной ниже таблице показаны обязательные свойства при активации роли каталога.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-130">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="ba8b4-131">Обязательный параметр</span><span class="sxs-lookup"><span data-stu-id="ba8b4-131">Required parameter</span></span> | <span data-ttu-id="ba8b4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ba8b4-132">Type</span></span> | <span data-ttu-id="ba8b4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ba8b4-133">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="ba8b4-134">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="ba8b4-134">roleTemplateId</span></span> | <span data-ttu-id="ba8b4-135">string</span><span class="sxs-lookup"><span data-stu-id="ba8b4-135">string</span></span> | <span data-ttu-id="ba8b4-p104">Идентификатор для объекта [directoryRoleTemplate](../resources/directoryroletemplate.md), который лежит в основе роли. Это единственное свойство, которое можно указать в запросе.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="ba8b4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba8b4-138">Response</span></span>

<span data-ttu-id="ba8b4-139">В случае успеха этот метод возвратит код отклика `201, Created` и объект [directoryRole](../resources/directoryrole.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-139">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba8b4-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ba8b4-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba8b4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba8b4-141">Request</span></span>

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
<span data-ttu-id="ba8b4-142">В теле запроса укажите описание объекта [directoryRole](../resources/directoryrole.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-142">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ba8b4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba8b4-143">Response</span></span>
<span data-ttu-id="ba8b4-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba8b4-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
