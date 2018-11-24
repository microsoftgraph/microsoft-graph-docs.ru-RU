# <a name="get-tab"></a><span data-ttu-id="cb794-101">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="cb794-101">Get tab</span></span>



<span data-ttu-id="cb794-102">Извлечение свойств и связи указанного [вкладки](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="cb794-102">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="cb794-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb794-103">Permissions</span></span>
<span data-ttu-id="cb794-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cb794-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb794-106">Permission type</span></span>      | <span data-ttu-id="cb794-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb794-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb794-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb794-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cb794-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb794-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb794-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb794-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb794-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb794-111">Not supported.</span></span>    |
|<span data-ttu-id="cb794-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb794-112">Application</span></span> | <span data-ttu-id="cb794-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb794-113">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="cb794-114">На данный момент только [делегированных разрешений](../../../concepts/permissions_reference.md) поддерживаются для этой операции.</span><span class="sxs-lookup"><span data-stu-id="cb794-114">Currently, only [delegated permissions](../../../concepts/permissions_reference.md) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="cb794-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb794-115">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb794-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb794-116">Optional query parameters</span></span>

<span data-ttu-id="cb794-117">Этот метод поддерживает $select и $разверните [Параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cb794-117">This method supports the $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb794-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb794-118">Request headers</span></span>
| <span data-ttu-id="cb794-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb794-119">Header</span></span>       | <span data-ttu-id="cb794-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cb794-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb794-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb794-121">Authorization</span></span>  | <span data-ttu-id="cb794-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb794-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb794-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb794-124">Request body</span></span>
<span data-ttu-id="cb794-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb794-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb794-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb794-126">Response</span></span>

<span data-ttu-id="cb794-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [tab](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb794-127">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb794-128">Пример</span><span class="sxs-lookup"><span data-stu-id="cb794-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cb794-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb794-129">Request</span></span>
<span data-ttu-id="cb794-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb794-130">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="cb794-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb794-131">Response</span></span>
<span data-ttu-id="cb794-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb794-132">The following is an example of the response.</span></span> 

><span data-ttu-id="cb794-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb794-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
