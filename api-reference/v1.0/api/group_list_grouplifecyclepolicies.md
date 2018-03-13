# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="b7520-101">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="b7520-101">List groupLifecyclePolicies</span></span>

<span data-ttu-id="b7520-102">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="b7520-102">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7520-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7520-103">Permissions</span></span>

<span data-ttu-id="b7520-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b7520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b7520-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7520-106">Permission type</span></span>      | <span data-ttu-id="b7520-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7520-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7520-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7520-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b7520-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7520-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="b7520-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7520-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7520-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7520-111">Not supported.</span></span>    |
|<span data-ttu-id="b7520-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7520-112">Application</span></span> | <span data-ttu-id="b7520-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7520-113">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7520-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7520-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7520-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7520-115">Optional query parameters</span></span>
<span data-ttu-id="b7520-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b7520-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7520-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7520-117">Request headers</span></span>
| <span data-ttu-id="b7520-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b7520-118">Name</span></span> | <span data-ttu-id="b7520-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b7520-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b7520-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7520-120">Authorization</span></span> | <span data-ttu-id="b7520-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7520-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7520-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7520-123">Request body</span></span>
<span data-ttu-id="b7520-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7520-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b7520-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7520-125">Response</span></span>
<span data-ttu-id="b7520-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b7520-126">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7520-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b7520-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b7520-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7520-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="b7520-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7520-129">Response</span></span>

<span data-ttu-id="b7520-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7520-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->