# <a name="delete-calendargroup"></a><span data-ttu-id="bd60e-101">Удаление объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="bd60e-101">Delete calendarGroup</span></span>

<span data-ttu-id="bd60e-102">Удаление группы календарей, отличной от стандартной.</span><span class="sxs-lookup"><span data-stu-id="bd60e-102">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd60e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd60e-103">Permissions</span></span>

<span data-ttu-id="bd60e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd60e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="bd60e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd60e-106">Permission type</span></span>                        | <span data-ttu-id="bd60e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd60e-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bd60e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd60e-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd60e-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd60e-109">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bd60e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd60e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd60e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd60e-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bd60e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd60e-112">Application</span></span>                            | <span data-ttu-id="bd60e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd60e-113">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bd60e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd60e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bd60e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd60e-115">Request headers</span></span>

| <span data-ttu-id="bd60e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="bd60e-116">Name</span></span>          | <span data-ttu-id="bd60e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="bd60e-117">Type</span></span>   | <span data-ttu-id="bd60e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="bd60e-118">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="bd60e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd60e-119">Authorization</span></span> | <span data-ttu-id="bd60e-120">string</span><span class="sxs-lookup"><span data-stu-id="bd60e-120">string</span></span> | <span data-ttu-id="bd60e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd60e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd60e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd60e-123">Request body</span></span>

<span data-ttu-id="bd60e-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd60e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd60e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd60e-125">Response</span></span>

<span data-ttu-id="bd60e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bd60e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd60e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bd60e-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bd60e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd60e-129">Request</span></span>

<span data-ttu-id="bd60e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd60e-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="bd60e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd60e-131">Response</span></span>

<span data-ttu-id="bd60e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd60e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
