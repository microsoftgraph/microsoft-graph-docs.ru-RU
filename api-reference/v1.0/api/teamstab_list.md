# <a name="list-tabs-in-channel"></a><span data-ttu-id="f3203-101">Список вкладок в канале</span><span class="sxs-lookup"><span data-stu-id="f3203-101">List tabs in channel</span></span>



<span data-ttu-id="f3203-102">Получить список [вкладок](../resources/teamstab.md) в указанный [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f3203-102">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f3203-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3203-103">Permissions</span></span>
<span data-ttu-id="f3203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f3203-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3203-106">Permission type</span></span>      | <span data-ttu-id="f3203-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3203-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3203-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3203-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f3203-109">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3203-109">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="f3203-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3203-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3203-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3203-111">Not supported.</span></span>    |
| <span data-ttu-id="f3203-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3203-112">Application</span></span>                            | <span data-ttu-id="f3203-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3203-113">Group.Read.All, Group.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="f3203-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3203-114">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3203-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3203-115">Optional query parameters</span></span>

<span data-ttu-id="f3203-116">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3203-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3203-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3203-117">Request headers</span></span>
| <span data-ttu-id="f3203-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3203-118">Header</span></span>       | <span data-ttu-id="f3203-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f3203-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3203-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3203-120">Authorization</span></span>  | <span data-ttu-id="f3203-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3203-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3203-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3203-123">Request body</span></span>
<span data-ttu-id="f3203-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3203-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3203-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3203-125">Response</span></span>
<span data-ttu-id="f3203-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [вкладок](../resources/teamstab.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f3203-126">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3203-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f3203-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f3203-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3203-128">Request</span></span>
<span data-ttu-id="f3203-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3203-129">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="f3203-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3203-130">Response</span></span>
<span data-ttu-id="f3203-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f3203-131">The following is an example of the response.</span></span>
><span data-ttu-id="f3203-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3203-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
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
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
