# <a name="delete-conversation"></a><span data-ttu-id="f0b73-101">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="f0b73-101">Delete conversation</span></span>
<span data-ttu-id="f0b73-102">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="f0b73-102">Delete conversation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0b73-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b73-103">Permissions</span></span>
<span data-ttu-id="f0b73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0b73-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b73-106">Permission type</span></span>      | <span data-ttu-id="f0b73-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0b73-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0b73-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0b73-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f0b73-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0b73-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0b73-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0b73-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0b73-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b73-111">Not supported.</span></span>    |
|<span data-ttu-id="f0b73-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0b73-112">Application</span></span> | <span data-ttu-id="f0b73-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b73-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0b73-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0b73-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0b73-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0b73-115">Request headers</span></span>
| <span data-ttu-id="f0b73-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f0b73-116">Name</span></span>       | <span data-ttu-id="f0b73-117">Тип</span><span class="sxs-lookup"><span data-stu-id="f0b73-117">Type</span></span> | <span data-ttu-id="f0b73-118">Описание</span><span class="sxs-lookup"><span data-stu-id="f0b73-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0b73-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0b73-119">Authorization</span></span>  | <span data-ttu-id="f0b73-120">string</span><span class="sxs-lookup"><span data-stu-id="f0b73-120">string</span></span>  | <span data-ttu-id="f0b73-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0b73-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0b73-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0b73-123">Request body</span></span>
<span data-ttu-id="f0b73-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0b73-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0b73-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b73-125">Response</span></span>
<span data-ttu-id="f0b73-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f0b73-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b73-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f0b73-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f0b73-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0b73-129">Request</span></span>
<span data-ttu-id="f0b73-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0b73-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="f0b73-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b73-131">Response</span></span>
<span data-ttu-id="f0b73-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0b73-132">The following is an example of the response.</span></span> 
><span data-ttu-id="f0b73-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f0b73-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f0b73-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0b73-134">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->