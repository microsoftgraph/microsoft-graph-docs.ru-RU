# <a name="delete-app-from-team"></a><span data-ttu-id="c38c6-101">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="c38c6-101">Delete app from team</span></span>



<span data-ttu-id="c38c6-102">Удаление [приложения](../resources/teamsappinstallation.md) из указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c38c6-102">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c38c6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c38c6-103">Permissions</span></span>
<span data-ttu-id="c38c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c38c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c38c6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c38c6-106">Permission type</span></span>      | <span data-ttu-id="c38c6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c38c6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c38c6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c38c6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c38c6-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c38c6-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c38c6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c38c6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c38c6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c38c6-111">Not supported.</span></span>    |
|<span data-ttu-id="c38c6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c38c6-112">Application</span></span> | <span data-ttu-id="c38c6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c38c6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c38c6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c38c6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c38c6-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c38c6-115">Request headers</span></span>
| <span data-ttu-id="c38c6-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c38c6-116">Header</span></span>       | <span data-ttu-id="c38c6-117">Значение</span><span class="sxs-lookup"><span data-stu-id="c38c6-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c38c6-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c38c6-118">Authorization</span></span>  | <span data-ttu-id="c38c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c38c6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c38c6-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c38c6-121">Request body</span></span>
<span data-ttu-id="c38c6-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c38c6-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c38c6-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="c38c6-123">Response</span></span>

<span data-ttu-id="c38c6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c38c6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c38c6-126">Пример</span><span class="sxs-lookup"><span data-stu-id="c38c6-126">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c38c6-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="c38c6-127">Request</span></span>
<span data-ttu-id="c38c6-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c38c6-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="c38c6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c38c6-129">Response</span></span>
<span data-ttu-id="c38c6-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c38c6-130">The following is an example of the response.</span></span> <span data-ttu-id="c38c6-131">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c38c6-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c38c6-132">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c38c6-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
