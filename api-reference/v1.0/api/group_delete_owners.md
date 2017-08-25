# <a name="remove-owner"></a><span data-ttu-id="1f303-101">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="1f303-101">Remove owner</span></span>

<span data-ttu-id="1f303-102">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="1f303-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f303-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f303-103">Permissions</span></span>
<span data-ttu-id="1f303-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1f303-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f303-106">Permission type</span></span>      | <span data-ttu-id="1f303-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f303-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1f303-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f303-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1f303-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f303-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="1f303-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f303-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f303-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f303-111">Not supported.</span></span>    | 
|<span data-ttu-id="1f303-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f303-112">Application</span></span> | <span data-ttu-id="1f303-113">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f303-113">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1f303-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f303-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1f303-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f303-115">Request headers</span></span>
| <span data-ttu-id="1f303-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1f303-116">Name</span></span>       | <span data-ttu-id="1f303-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1f303-117">Type</span></span> | <span data-ttu-id="1f303-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1f303-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f303-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f303-119">Authorization</span></span>  | <span data-ttu-id="1f303-120">string</span><span class="sxs-lookup"><span data-stu-id="1f303-120">string</span></span>  | <span data-ttu-id="1f303-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f303-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f303-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f303-123">Request body</span></span>
<span data-ttu-id="1f303-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f303-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f303-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f303-125">Response</span></span>

<span data-ttu-id="1f303-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1f303-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f303-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1f303-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f303-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f303-129">Request</span></span>
<span data-ttu-id="1f303-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f303-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="1f303-131">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="1f303-131">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="1f303-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f303-132">Response</span></span>
<span data-ttu-id="1f303-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1f303-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
