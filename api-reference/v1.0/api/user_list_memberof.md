# <a name="list-memberof"></a><span data-ttu-id="d3acd-101">Список свойств memberOf</span><span class="sxs-lookup"><span data-stu-id="d3acd-101">List memberOf</span></span>

<span data-ttu-id="d3acd-102">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="d3acd-102">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d3acd-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3acd-103">Permissions</span></span>
<span data-ttu-id="d3acd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3acd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3acd-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3acd-106">Permission type</span></span>      | <span data-ttu-id="d3acd-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3acd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3acd-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3acd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d3acd-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3acd-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d3acd-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3acd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3acd-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3acd-111">Not supported.</span></span>    |
|<span data-ttu-id="d3acd-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3acd-112">Application</span></span> | <span data-ttu-id="d3acd-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3acd-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3acd-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3acd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3acd-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3acd-115">Optional query parameters</span></span>
<span data-ttu-id="d3acd-p102">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика ($filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="d3acd-p102">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="d3acd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3acd-118">Request headers</span></span>
| <span data-ttu-id="d3acd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3acd-119">Header</span></span>       | <span data-ttu-id="d3acd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d3acd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3acd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3acd-121">Authorization</span></span>  | <span data-ttu-id="d3acd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3acd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3acd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d3acd-124">Accept</span></span>  | <span data-ttu-id="d3acd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3acd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3acd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3acd-126">Request body</span></span>
<span data-ttu-id="d3acd-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3acd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3acd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3acd-128">Response</span></span>

<span data-ttu-id="d3acd-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3acd-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3acd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d3acd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3acd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3acd-131">Request</span></span>
<span data-ttu-id="d3acd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3acd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="d3acd-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3acd-133">Response</span></span>
<span data-ttu-id="d3acd-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d3acd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
