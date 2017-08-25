# <a name="update-calendargroup"></a><span data-ttu-id="6a91f-101">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="6a91f-101">Update calendargroup</span></span>

<span data-ttu-id="6a91f-102">Обновление свойств объекта calendargroup.</span><span class="sxs-lookup"><span data-stu-id="6a91f-102">Update the properties of calendargroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a91f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a91f-103">Permissions</span></span>
<span data-ttu-id="6a91f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a91f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a91f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a91f-106">Permission type</span></span>      | <span data-ttu-id="6a91f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a91f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6a91f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a91f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6a91f-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a91f-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="6a91f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a91f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a91f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a91f-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="6a91f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a91f-112">Application</span></span> | <span data-ttu-id="6a91f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a91f-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6a91f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a91f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6a91f-115">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a91f-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6a91f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a91f-116">Request headers</span></span>
| <span data-ttu-id="6a91f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a91f-117">Header</span></span>       | <span data-ttu-id="6a91f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="6a91f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a91f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a91f-119">Authorization</span></span>  | <span data-ttu-id="6a91f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a91f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6a91f-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a91f-122">Content-Type</span></span>  | <span data-ttu-id="6a91f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a91f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a91f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a91f-125">Request body</span></span>
<span data-ttu-id="6a91f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6a91f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6a91f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a91f-129">Property</span></span>     | <span data-ttu-id="6a91f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6a91f-130">Type</span></span>   |<span data-ttu-id="6a91f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6a91f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a91f-132">name</span><span class="sxs-lookup"><span data-stu-id="6a91f-132">name</span></span>|<span data-ttu-id="6a91f-133">String</span><span class="sxs-lookup"><span data-stu-id="6a91f-133">String</span></span>|<span data-ttu-id="6a91f-134">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="6a91f-134">The group name.</span></span>|

## <a name="response"></a><span data-ttu-id="6a91f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a91f-135">Response</span></span>

<span data-ttu-id="6a91f-136">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a91f-136">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a91f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6a91f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a91f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a91f-138">Request</span></span>
<span data-ttu-id="6a91f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a91f-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="6a91f-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a91f-140">Response</span></span>
<span data-ttu-id="6a91f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6a91f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
