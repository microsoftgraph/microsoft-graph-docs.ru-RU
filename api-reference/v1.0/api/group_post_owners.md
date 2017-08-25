# <a name="add-group-owner"></a><span data-ttu-id="58ac0-101">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="58ac0-101">Add group owner</span></span>
<span data-ttu-id="58ac0-p101">Добавление пользователя в качестве владельца группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="58ac0-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58ac0-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58ac0-104">Permissions</span></span>
<span data-ttu-id="58ac0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58ac0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="58ac0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58ac0-107">Permission type</span></span>      | <span data-ttu-id="58ac0-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58ac0-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="58ac0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58ac0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="58ac0-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58ac0-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="58ac0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58ac0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58ac0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58ac0-112">Not supported.</span></span>    | 
|<span data-ttu-id="58ac0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58ac0-113">Application</span></span> | <span data-ttu-id="58ac0-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58ac0-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="58ac0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58ac0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="58ac0-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58ac0-116">Request headers</span></span>
| <span data-ttu-id="58ac0-117">Имя</span><span class="sxs-lookup"><span data-stu-id="58ac0-117">Name</span></span>       | <span data-ttu-id="58ac0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="58ac0-118">Type</span></span> | <span data-ttu-id="58ac0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="58ac0-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58ac0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="58ac0-120">Authorization</span></span>  | <span data-ttu-id="58ac0-121">string</span><span class="sxs-lookup"><span data-stu-id="58ac0-121">string</span></span>  | <span data-ttu-id="58ac0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58ac0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58ac0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58ac0-124">Request body</span></span>
<span data-ttu-id="58ac0-125">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58ac0-125">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="58ac0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="58ac0-126">Response</span></span>

<span data-ttu-id="58ac0-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="58ac0-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58ac0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="58ac0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58ac0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="58ac0-130">Request</span></span>
<span data-ttu-id="58ac0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58ac0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="58ac0-132">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58ac0-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="58ac0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="58ac0-133">Response</span></span>
<span data-ttu-id="58ac0-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="58ac0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
