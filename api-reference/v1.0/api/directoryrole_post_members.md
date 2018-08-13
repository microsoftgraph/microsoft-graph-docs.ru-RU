# <a name="add-directory-role-member"></a><span data-ttu-id="1aa1e-101">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="1aa1e-101">Add directory role member</span></span>

<span data-ttu-id="1aa1e-102">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-102">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="1aa1e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa1e-103">Permissions</span></span>
<span data-ttu-id="1aa1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1aa1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1aa1e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa1e-106">Permission type</span></span>      | <span data-ttu-id="1aa1e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aa1e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aa1e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aa1e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1aa1e-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1aa1e-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1aa1e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aa1e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aa1e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-111">Not supported.</span></span>    |
|<span data-ttu-id="1aa1e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aa1e-112">Application</span></span> | <span data-ttu-id="1aa1e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aa1e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aa1e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="1aa1e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aa1e-115">Request headers</span></span>
| <span data-ttu-id="1aa1e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1aa1e-116">Name</span></span>       | <span data-ttu-id="1aa1e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1aa1e-117">Type</span></span> | <span data-ttu-id="1aa1e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa1e-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1aa1e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aa1e-119">Authorization</span></span>  | <span data-ttu-id="1aa1e-120">string</span><span class="sxs-lookup"><span data-stu-id="1aa1e-120">string</span></span>  | <span data-ttu-id="1aa1e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1aa1e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1aa1e-123">Content-Type</span></span>  | <span data-ttu-id="1aa1e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1aa1e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1aa1e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1aa1e-125">Request body</span></span>
<span data-ttu-id="1aa1e-126">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="1aa1e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aa1e-127">Response</span></span>

<span data-ttu-id="1aa1e-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1aa1e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1aa1e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1aa1e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aa1e-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="1aa1e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aa1e-131">Response</span></span>
<span data-ttu-id="1aa1e-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1aa1e-132">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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