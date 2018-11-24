# <a name="get-team"></a><span data-ttu-id="7bd4f-101">Получение группы</span><span class="sxs-lookup"><span data-stu-id="7bd4f-101">Get team</span></span>



<span data-ttu-id="7bd4f-102">Извлечение свойств и связи из указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7bd4f-102">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bd4f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bd4f-103">Permissions</span></span>
<span data-ttu-id="7bd4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bd4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7bd4f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bd4f-106">Permission type</span></span>      | <span data-ttu-id="7bd4f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bd4f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bd4f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bd4f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7bd4f-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd4f-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bd4f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bd4f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bd4f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-111">Not supported.</span></span>    |
|<span data-ttu-id="7bd4f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bd4f-112">Application</span></span> | <span data-ttu-id="7bd4f-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd4f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7bd4f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bd4f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bd4f-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7bd4f-115">Optional query parameters</span></span>
<span data-ttu-id="7bd4f-116">Этот метод поддерживает $select и $разверните [Параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-116">This method supports the $select and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bd4f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bd4f-117">Request headers</span></span>
| <span data-ttu-id="7bd4f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bd4f-118">Header</span></span>       | <span data-ttu-id="7bd4f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7bd4f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7bd4f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bd4f-120">Authorization</span></span>  | <span data-ttu-id="7bd4f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7bd4f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bd4f-123">Request body</span></span>
<span data-ttu-id="7bd4f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bd4f-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bd4f-125">Response</span></span>

<span data-ttu-id="7bd4f-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объекта [группы](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-126">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bd4f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7bd4f-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7bd4f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bd4f-128">Request</span></span>
<span data-ttu-id="7bd4f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="7bd4f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bd4f-130">Response</span></span>
<span data-ttu-id="7bd4f-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-131">The following is an example of the response.</span></span> 

><span data-ttu-id="7bd4f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7bd4f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
