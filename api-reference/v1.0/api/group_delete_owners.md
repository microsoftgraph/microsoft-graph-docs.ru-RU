# <a name="remove-owner"></a><span data-ttu-id="28d00-101">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="28d00-101">Remove owner</span></span>
<span data-ttu-id="28d00-102">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="28d00-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="28d00-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28d00-103">Permissions</span></span>
<span data-ttu-id="28d00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="28d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="28d00-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28d00-106">Permission type</span></span>      | <span data-ttu-id="28d00-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28d00-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28d00-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28d00-108">Delegated (work or school account)</span></span> | <span data-ttu-id="28d00-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28d00-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28d00-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28d00-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d00-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d00-111">Not supported.</span></span>    |
|<span data-ttu-id="28d00-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28d00-112">Application</span></span> | <span data-ttu-id="28d00-113">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d00-113">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28d00-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28d00-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="28d00-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28d00-115">Request headers</span></span>
| <span data-ttu-id="28d00-116">Имя</span><span class="sxs-lookup"><span data-stu-id="28d00-116">Name</span></span>       | <span data-ttu-id="28d00-117">Тип</span><span class="sxs-lookup"><span data-stu-id="28d00-117">Type</span></span> | <span data-ttu-id="28d00-118">Описание</span><span class="sxs-lookup"><span data-stu-id="28d00-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28d00-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="28d00-119">Authorization</span></span>  | <span data-ttu-id="28d00-120">string</span><span class="sxs-lookup"><span data-stu-id="28d00-120">string</span></span>  | <span data-ttu-id="28d00-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28d00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28d00-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28d00-123">Request body</span></span>
<span data-ttu-id="28d00-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28d00-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d00-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d00-125">Response</span></span>
<span data-ttu-id="28d00-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="28d00-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d00-128">Пример</span><span class="sxs-lookup"><span data-stu-id="28d00-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="28d00-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="28d00-129">Request</span></span>
<span data-ttu-id="28d00-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28d00-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="28d00-131">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="28d00-131">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="28d00-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d00-132">Response</span></span>
<span data-ttu-id="28d00-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28d00-133">The following is an example of the response.</span></span>
><span data-ttu-id="28d00-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28d00-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="28d00-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28d00-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
