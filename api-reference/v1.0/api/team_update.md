# <a name="update-team"></a><span data-ttu-id="fbb4e-101">Группа обновления</span><span class="sxs-lookup"><span data-stu-id="fbb4e-101">Update team</span></span>



<span data-ttu-id="fbb4e-102">Обновление свойств указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fbb4e-102">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbb4e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb4e-103">Permissions</span></span>
<span data-ttu-id="fbb4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fbb4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="fbb4e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb4e-106">Permission type</span></span>      | <span data-ttu-id="fbb4e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbb4e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbb4e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbb4e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fbb4e-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb4e-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbb4e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbb4e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbb4e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-111">Not supported.</span></span>    |
|<span data-ttu-id="fbb4e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbb4e-112">Application</span></span> | <span data-ttu-id="fbb4e-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb4e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="fbb4e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbb4e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fbb4e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbb4e-115">Request headers</span></span>
| <span data-ttu-id="fbb4e-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbb4e-116">Header</span></span>       | <span data-ttu-id="fbb4e-117">Значение</span><span class="sxs-lookup"><span data-stu-id="fbb4e-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbb4e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbb4e-118">Authorization</span></span>  | <span data-ttu-id="fbb4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fbb4e-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbb4e-121">Content-Type</span></span>  | <span data-ttu-id="fbb4e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fbb4e-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbb4e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbb4e-123">Request body</span></span>
<span data-ttu-id="fbb4e-124">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="fbb4e-124">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fbb4e-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbb4e-125">Response</span></span>

<span data-ttu-id="fbb4e-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fbb4e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fbb4e-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fbb4e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbb4e-128">Request</span></span>
<span data-ttu-id="fbb4e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbb4e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="fbb4e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbb4e-130">Response</span></span>
<!-- {
  "blockType": "response",
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
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
