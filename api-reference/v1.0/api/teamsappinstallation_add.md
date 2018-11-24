# <a name="add-app-to-team"></a><span data-ttu-id="b4231-101">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="b4231-101">Add app to team</span></span>



<span data-ttu-id="b4231-102">Пакет [приложения](../resources/teamsapp.md) для указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b4231-102">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4231-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4231-103">Permissions</span></span>
<span data-ttu-id="b4231-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4231-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4231-106">Permission type</span></span>      | <span data-ttu-id="b4231-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4231-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4231-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4231-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b4231-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4231-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4231-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4231-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4231-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4231-111">Not supported.</span></span>    |
|<span data-ttu-id="b4231-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4231-112">Application</span></span> | <span data-ttu-id="b4231-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4231-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4231-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4231-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="b4231-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4231-115">Request headers</span></span>
| <span data-ttu-id="b4231-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4231-116">Header</span></span>       | <span data-ttu-id="b4231-117">Значение</span><span class="sxs-lookup"><span data-stu-id="b4231-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4231-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4231-118">Authorization</span></span>  | <span data-ttu-id="b4231-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4231-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4231-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4231-121">Request body</span></span>

| <span data-ttu-id="b4231-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4231-122">Property</span></span>     | <span data-ttu-id="b4231-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b4231-123">Type</span></span>   |<span data-ttu-id="b4231-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b4231-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4231-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b4231-125">teamsApp</span></span>| [<span data-ttu-id="b4231-126">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b4231-126">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="b4231-127">Чтобы добавить приложение.</span><span class="sxs-lookup"><span data-stu-id="b4231-127">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="b4231-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4231-128">Response</span></span>

<span data-ttu-id="b4231-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b4231-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4231-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b4231-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b4231-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4231-131">Request</span></span>
<span data-ttu-id="b4231-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4231-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="b4231-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4231-133">Response</span></span>
<span data-ttu-id="b4231-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4231-134">The following is an example of the response.</span></span> <span data-ttu-id="b4231-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b4231-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b4231-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4231-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
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

## <a name="see-also"></a><span data-ttu-id="b4231-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b4231-137">See also</span></span>

