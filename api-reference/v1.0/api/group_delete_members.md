# <a name="remove-member"></a><span data-ttu-id="404ee-101">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="404ee-101">Remove member</span></span>

<span data-ttu-id="404ee-p101">С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="404ee-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="404ee-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="404ee-104">Permissions</span></span>
<span data-ttu-id="404ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="404ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="404ee-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="404ee-107">Permission type</span></span>      | <span data-ttu-id="404ee-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="404ee-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="404ee-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="404ee-109">Delegated (work or school account)</span></span> | <span data-ttu-id="404ee-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="404ee-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="404ee-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="404ee-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="404ee-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="404ee-112">Not supported.</span></span>    | 
|<span data-ttu-id="404ee-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="404ee-113">Application</span></span> | <span data-ttu-id="404ee-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="404ee-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="404ee-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="404ee-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="404ee-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="404ee-116">Request headers</span></span>
| <span data-ttu-id="404ee-117">Имя</span><span class="sxs-lookup"><span data-stu-id="404ee-117">Name</span></span>       | <span data-ttu-id="404ee-118">Тип</span><span class="sxs-lookup"><span data-stu-id="404ee-118">Type</span></span> | <span data-ttu-id="404ee-119">Описание</span><span class="sxs-lookup"><span data-stu-id="404ee-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="404ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="404ee-120">Authorization</span></span>  | <span data-ttu-id="404ee-121">string</span><span class="sxs-lookup"><span data-stu-id="404ee-121">string</span></span>  | <span data-ttu-id="404ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="404ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="404ee-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="404ee-124">Request body</span></span>
<span data-ttu-id="404ee-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="404ee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="404ee-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="404ee-126">Response</span></span>

<span data-ttu-id="404ee-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="404ee-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="404ee-129">Пример</span><span class="sxs-lookup"><span data-stu-id="404ee-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="404ee-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="404ee-130">Request</span></span>
<span data-ttu-id="404ee-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="404ee-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="404ee-132">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="404ee-132">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="404ee-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="404ee-133">Response</span></span>
<span data-ttu-id="404ee-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="404ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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