# <a name="add-member"></a><span data-ttu-id="69686-101">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="69686-101">Add member</span></span>

<span data-ttu-id="69686-p101">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**. Вы можете добавлять пользователей или другие группы. Важно! В группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="69686-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="69686-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69686-105">Permissions</span></span>
<span data-ttu-id="69686-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69686-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="69686-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69686-108">Permission type</span></span>      | <span data-ttu-id="69686-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69686-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="69686-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69686-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69686-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69686-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="69686-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69686-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69686-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69686-113">Not supported.</span></span>    | 
|<span data-ttu-id="69686-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69686-114">Application</span></span> | <span data-ttu-id="69686-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69686-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="69686-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69686-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="69686-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69686-117">Request headers</span></span>
| <span data-ttu-id="69686-118">Имя</span><span class="sxs-lookup"><span data-stu-id="69686-118">Name</span></span>       | <span data-ttu-id="69686-119">Тип</span><span class="sxs-lookup"><span data-stu-id="69686-119">Type</span></span> | <span data-ttu-id="69686-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69686-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69686-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69686-121">Authorization</span></span>  | <span data-ttu-id="69686-122">string</span><span class="sxs-lookup"><span data-stu-id="69686-122">string</span></span>  | <span data-ttu-id="69686-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69686-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69686-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69686-125">Request body</span></span>
<span data-ttu-id="69686-126">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69686-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="69686-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="69686-127">Response</span></span>

<span data-ttu-id="69686-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="69686-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69686-130">Пример</span><span class="sxs-lookup"><span data-stu-id="69686-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69686-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="69686-131">Request</span></span>
<span data-ttu-id="69686-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69686-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="69686-133">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69686-133">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="69686-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="69686-134">Response</span></span>
<span data-ttu-id="69686-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="69686-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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