# <a name="patch-channel"></a><span data-ttu-id="79611-101">Исправление канала</span><span class="sxs-lookup"><span data-stu-id="79611-101">Patch channel</span></span>



<span data-ttu-id="79611-102">Обновляет свойства указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="79611-102">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="79611-103">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="79611-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="79611-104">Дополнительные сведения см [Известные проблемы списка](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="79611-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="79611-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79611-105">Permissions</span></span>
<span data-ttu-id="79611-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79611-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79611-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79611-108">Permission type</span></span>      | <span data-ttu-id="79611-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79611-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79611-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79611-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79611-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79611-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="79611-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79611-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79611-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79611-113">Not supported.</span></span>    |
|<span data-ttu-id="79611-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79611-114">Application</span></span> | <span data-ttu-id="79611-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79611-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79611-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79611-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79611-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79611-117">Request headers</span></span>
| <span data-ttu-id="79611-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79611-118">Header</span></span>       | <span data-ttu-id="79611-119">Значение</span><span class="sxs-lookup"><span data-stu-id="79611-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79611-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79611-120">Authorization</span></span>  | <span data-ttu-id="79611-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79611-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79611-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79611-123">Content-Type</span></span>  | <span data-ttu-id="79611-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79611-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79611-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79611-125">Request body</span></span>
<span data-ttu-id="79611-126">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="79611-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="79611-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="79611-127">Response</span></span>

<span data-ttu-id="79611-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79611-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79611-129">Пример</span><span class="sxs-lookup"><span data-stu-id="79611-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79611-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="79611-130">Request</span></span>
<span data-ttu-id="79611-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79611-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="79611-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="79611-132">Response</span></span>
<span data-ttu-id="79611-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="79611-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
