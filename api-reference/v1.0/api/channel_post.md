# <a name="create-channel"></a><span data-ttu-id="659f2-101">Создание канала</span><span class="sxs-lookup"><span data-stu-id="659f2-101">Create Channel</span></span>



<span data-ttu-id="659f2-102">Создайте новый [канал](../resources/channel.md) в группы разработчиков Microsoft, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="659f2-102">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="659f2-103">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="659f2-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="659f2-104">Дополнительные сведения см [Известные проблемы списка](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="659f2-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="659f2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="659f2-105">Permissions</span></span>
<span data-ttu-id="659f2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="659f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="659f2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="659f2-108">Permission type</span></span>      | <span data-ttu-id="659f2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="659f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="659f2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="659f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="659f2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659f2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="659f2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="659f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="659f2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="659f2-113">Not supported.</span></span>    |
|<span data-ttu-id="659f2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="659f2-114">Application</span></span> | <span data-ttu-id="659f2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659f2-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="659f2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="659f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="659f2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="659f2-117">Request headers</span></span>
| <span data-ttu-id="659f2-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="659f2-118">Header</span></span>       | <span data-ttu-id="659f2-119">Значение</span><span class="sxs-lookup"><span data-stu-id="659f2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="659f2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="659f2-120">Authorization</span></span>  | <span data-ttu-id="659f2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="659f2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="659f2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="659f2-123">Content-Type</span></span>  | <span data-ttu-id="659f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="659f2-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="659f2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="659f2-125">Request body</span></span>
<span data-ttu-id="659f2-126">В тексте запроса укажите представление JSON объекта [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="659f2-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="659f2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="659f2-127">Response</span></span>

<span data-ttu-id="659f2-128">Успешно завершена, этот метод возвращает `201 Created` объект [канала](../resources/channel.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="659f2-128">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="659f2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="659f2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="659f2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="659f2-130">Request</span></span>
<span data-ttu-id="659f2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="659f2-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="659f2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="659f2-132">Response</span></span>
<span data-ttu-id="659f2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="659f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
