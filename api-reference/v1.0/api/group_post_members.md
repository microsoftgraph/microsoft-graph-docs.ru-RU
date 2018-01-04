# <a name="add-member"></a><span data-ttu-id="c708e-101">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="c708e-101">Add member</span></span>
<span data-ttu-id="c708e-102">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="c708e-102">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

<span data-ttu-id="c708e-103">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="c708e-103">You can add users or other groups.</span></span> <span data-ttu-id="c708e-104">Важно! В Группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="c708e-104">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c708e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c708e-105">Permissions</span></span>
<span data-ttu-id="c708e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c708e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c708e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c708e-108">Permission type</span></span>      | <span data-ttu-id="c708e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c708e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c708e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c708e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c708e-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c708e-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c708e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c708e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c708e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c708e-113">Not supported.</span></span>    |
|<span data-ttu-id="c708e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c708e-114">Application</span></span> | <span data-ttu-id="c708e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c708e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c708e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c708e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c708e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c708e-117">Request headers</span></span>
| <span data-ttu-id="c708e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c708e-118">Name</span></span>       | <span data-ttu-id="c708e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c708e-119">Type</span></span> | <span data-ttu-id="c708e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c708e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c708e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c708e-121">Authorization</span></span>  | <span data-ttu-id="c708e-122">string</span><span class="sxs-lookup"><span data-stu-id="c708e-122">string</span></span>  | <span data-ttu-id="c708e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c708e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c708e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c708e-125">Request body</span></span>
<span data-ttu-id="c708e-126">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c708e-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c708e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708e-127">Response</span></span>
<span data-ttu-id="c708e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c708e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c708e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c708e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c708e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c708e-131">Request</span></span>
<span data-ttu-id="c708e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c708e-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="c708e-133">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c708e-133">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="c708e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708e-134">Response</span></span>
<span data-ttu-id="c708e-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c708e-135">The following is an example of the response.</span></span>
><span data-ttu-id="c708e-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c708e-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c708e-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c708e-137">All the properties will be returned from an actual call.</span></span>
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