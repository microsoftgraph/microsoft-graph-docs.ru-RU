# <a name="delete-calendargroup"></a><span data-ttu-id="65b51-101">Удаление объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="65b51-101">Delete calendarGroup</span></span>

<span data-ttu-id="65b51-102">Удаление группы календарей, отличной от стандартной.</span><span class="sxs-lookup"><span data-stu-id="65b51-102">Delete a calendar group other than the default calendar group.</span></span>

<span data-ttu-id="65b51-p101">**Примечание**. Outlook.com поддерживает только группу календарей по умолчанию, доступную по ссылке /me/calendars. Удалить группу календарей в Outlook.com невозможно.</span><span class="sxs-lookup"><span data-stu-id="65b51-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the /me/calendars shortcut. You cannot delete any calendar group in Outlook.com.</span></span>

## <a name="permissions"></a><span data-ttu-id="65b51-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65b51-105">Permissions</span></span>
<span data-ttu-id="65b51-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65b51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65b51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65b51-108">Permission type</span></span>      | <span data-ttu-id="65b51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65b51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65b51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65b51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65b51-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65b51-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="65b51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65b51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b51-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65b51-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="65b51-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65b51-114">Application</span></span> | <span data-ttu-id="65b51-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65b51-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="65b51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65b51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="65b51-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65b51-117">Request headers</span></span>
| <span data-ttu-id="65b51-118">Имя</span><span class="sxs-lookup"><span data-stu-id="65b51-118">Name</span></span>       | <span data-ttu-id="65b51-119">Тип</span><span class="sxs-lookup"><span data-stu-id="65b51-119">Type</span></span> | <span data-ttu-id="65b51-120">Описание</span><span class="sxs-lookup"><span data-stu-id="65b51-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="65b51-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b51-121">Authorization</span></span>  | <span data-ttu-id="65b51-122">string</span><span class="sxs-lookup"><span data-stu-id="65b51-122">string</span></span>  | <span data-ttu-id="65b51-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65b51-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65b51-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65b51-125">Request body</span></span>
<span data-ttu-id="65b51-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65b51-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65b51-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b51-127">Response</span></span>

<span data-ttu-id="65b51-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="65b51-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65b51-130">Пример</span><span class="sxs-lookup"><span data-stu-id="65b51-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65b51-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="65b51-131">Request</span></span>
<span data-ttu-id="65b51-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65b51-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="65b51-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="65b51-133">Response</span></span>
<span data-ttu-id="65b51-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="65b51-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
