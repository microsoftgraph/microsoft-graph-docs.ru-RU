# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="71786-101">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="71786-101">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="71786-102">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71786-102">Retrieve the properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71786-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71786-103">Permissions</span></span>

<span data-ttu-id="71786-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71786-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71786-106">Permission type</span></span>      | <span data-ttu-id="71786-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71786-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71786-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71786-108">Delegated (work or school account)</span></span> | <span data-ttu-id="71786-109">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71786-109">Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="71786-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71786-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71786-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71786-111">Not supported.</span></span>    |
|<span data-ttu-id="71786-112">Для приложения</span><span class="sxs-lookup"><span data-stu-id="71786-112">Application</span></span> | <span data-ttu-id="71786-113">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71786-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71786-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71786-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71786-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71786-115">Optional query parameters</span></span>
<span data-ttu-id="71786-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71786-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71786-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71786-117">Request headers</span></span>
| <span data-ttu-id="71786-118">Имя</span><span class="sxs-lookup"><span data-stu-id="71786-118">Name</span></span> | <span data-ttu-id="71786-119">Описание</span><span class="sxs-lookup"><span data-stu-id="71786-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="71786-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71786-120">Authorization</span></span> | <span data-ttu-id="71786-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71786-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71786-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71786-123">Request body</span></span>
<span data-ttu-id="71786-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71786-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71786-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="71786-125">Response</span></span>
<span data-ttu-id="71786-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71786-126">If successful, this method returns a `200 OK` response code and a [group](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71786-127">Пример</span><span class="sxs-lookup"><span data-stu-id="71786-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71786-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="71786-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="71786-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71786-129">Response</span></span>

<span data-ttu-id="71786-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71786-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->