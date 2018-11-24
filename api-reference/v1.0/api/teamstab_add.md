# <a name="add-tab-to-channel"></a><span data-ttu-id="2552c-101">Добавление вкладки канала</span><span class="sxs-lookup"><span data-stu-id="2552c-101">Add tab to channel</span></span>



<span data-ttu-id="2552c-102">Добавляет (PIN) [вкладки](../resources/teamstab.md) для указанного [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2552c-102">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="2552c-103">Соответствующие приложения уже должен быть [установлен в группе](../api/teamsappinstallation_add.md).</span><span class="sxs-lookup"><span data-stu-id="2552c-103">The corresponding app must already be [installed in the team](../api/teamsappinstallation_add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2552c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2552c-104">Permissions</span></span>
<span data-ttu-id="2552c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2552c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2552c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2552c-107">Permission type</span></span>      | <span data-ttu-id="2552c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2552c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2552c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2552c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2552c-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2552c-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2552c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2552c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2552c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2552c-112">Not supported.</span></span>    |
| <span data-ttu-id="2552c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2552c-113">Application</span></span>                            | <span data-ttu-id="2552c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2552c-114">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2552c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2552c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="2552c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2552c-116">Request headers</span></span>
| <span data-ttu-id="2552c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2552c-117">Header</span></span>       | <span data-ttu-id="2552c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2552c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2552c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2552c-119">Authorization</span></span>  | <span data-ttu-id="2552c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2552c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2552c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2552c-122">Request body</span></span>

<span data-ttu-id="2552c-123">[TeamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="2552c-123">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="2552c-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="2552c-124">Response</span></span>

<span data-ttu-id="2552c-125">В случае успешного выполнения этот метод возвращает код отклика `201 OK`.</span><span class="sxs-lookup"><span data-stu-id="2552c-125">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2552c-126">Пример</span><span class="sxs-lookup"><span data-stu-id="2552c-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2552c-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="2552c-127">Request</span></span>

<span data-ttu-id="2552c-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2552c-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="2552c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2552c-129">Response</span></span>

<span data-ttu-id="2552c-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2552c-130">The following is an example of the response.</span></span> <span data-ttu-id="2552c-131">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2552c-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2552c-132">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2552c-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "name": "My Contoso Tab",
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

## <a name="see-also"></a><span data-ttu-id="2552c-133">См. также</span><span class="sxs-lookup"><span data-stu-id="2552c-133">See also</span></span>

[<span data-ttu-id="2552c-134">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="2552c-134">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
