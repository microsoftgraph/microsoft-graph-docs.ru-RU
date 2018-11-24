# <a name="update-tab"></a><span data-ttu-id="156d5-101">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="156d5-101">Update tab</span></span>



<span data-ttu-id="156d5-102">Обновляет свойства указанной [вкладки](../resources/teamstab.md). Это можно использовать для настройки содержимого вкладки.</span><span class="sxs-lookup"><span data-stu-id="156d5-102">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="156d5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="156d5-103">Permissions</span></span>
<span data-ttu-id="156d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="156d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="156d5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="156d5-106">Permission type</span></span>      | <span data-ttu-id="156d5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="156d5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="156d5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="156d5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="156d5-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="156d5-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="156d5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="156d5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="156d5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="156d5-111">Not supported.</span></span>    |
|<span data-ttu-id="156d5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="156d5-112">Application</span></span>                            | <span data-ttu-id="156d5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="156d5-113">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="156d5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="156d5-114">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="156d5-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="156d5-115">Request headers</span></span>
| <span data-ttu-id="156d5-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="156d5-116">Header</span></span>       | <span data-ttu-id="156d5-117">Значение</span><span class="sxs-lookup"><span data-stu-id="156d5-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="156d5-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="156d5-118">Authorization</span></span>  | <span data-ttu-id="156d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="156d5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="156d5-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="156d5-121">Content-Type</span></span>  | <span data-ttu-id="156d5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="156d5-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="156d5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="156d5-123">Request body</span></span>
<span data-ttu-id="156d5-124">В тексте запроса укажите представление JSON объекта [вкладки](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="156d5-124">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="156d5-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="156d5-125">Response</span></span>

<span data-ttu-id="156d5-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="156d5-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="156d5-127">Пример</span><span class="sxs-lookup"><span data-stu-id="156d5-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="156d5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="156d5-128">Request</span></span>
<span data-ttu-id="156d5-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="156d5-129">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="156d5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="156d5-130">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

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

## <a name="see-also"></a><span data-ttu-id="156d5-131">См. также</span><span class="sxs-lookup"><span data-stu-id="156d5-131">See also</span></span>

[<span data-ttu-id="156d5-132">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="156d5-132">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
