# <a name="list-directoryroles"></a><span data-ttu-id="224b0-101">Список объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="224b0-101">List directoryRoles</span></span>

<span data-ttu-id="224b0-102">Список ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="224b0-102">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="224b0-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="224b0-103">Permissions</span></span>
<span data-ttu-id="224b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="224b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="224b0-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="224b0-106">Permission type</span></span>      | <span data-ttu-id="224b0-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="224b0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="224b0-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="224b0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="224b0-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="224b0-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="224b0-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="224b0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="224b0-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="224b0-111">Not supported.</span></span>    |
|<span data-ttu-id="224b0-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="224b0-112">Application</span></span> | <span data-ttu-id="224b0-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="224b0-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="224b0-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="224b0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="224b0-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="224b0-115">Optional query parameters</span></span>
<span data-ttu-id="224b0-116">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="224b0-116">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="224b0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="224b0-117">Request headers</span></span>
| <span data-ttu-id="224b0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="224b0-118">Name</span></span>       | <span data-ttu-id="224b0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="224b0-119">Type</span></span> | <span data-ttu-id="224b0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="224b0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="224b0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="224b0-121">Authorization</span></span>  | <span data-ttu-id="224b0-122">string</span><span class="sxs-lookup"><span data-stu-id="224b0-122">string</span></span>  | <span data-ttu-id="224b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="224b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="224b0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="224b0-125">Request body</span></span>
<span data-ttu-id="224b0-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="224b0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="224b0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="224b0-127">Response</span></span>

<span data-ttu-id="224b0-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="224b0-128">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="224b0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="224b0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="224b0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="224b0-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="224b0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="224b0-131">Response</span></span>
<span data-ttu-id="224b0-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="224b0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
