# <a name="update-a-group-setting"></a><span data-ttu-id="5b728-101">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="5b728-101">Update a group setting</span></span>

<span data-ttu-id="5b728-102">Обновление свойств для указанных объектов параметров группы.</span><span class="sxs-lookup"><span data-stu-id="5b728-102">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b728-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b728-103">Permissions</span></span>

<span data-ttu-id="5b728-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5b728-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b728-106">Permission type</span></span>      | <span data-ttu-id="5b728-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b728-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="5b728-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b728-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5b728-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b728-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="5b728-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b728-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b728-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b728-111">Not supported.</span></span>    | 
|<span data-ttu-id="5b728-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b728-112">Application</span></span> | <span data-ttu-id="5b728-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b728-113">Directory.ReadWrite.All</span></span> | 


## <a name="http-request"></a><span data-ttu-id="5b728-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b728-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5b728-115">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="5b728-115">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5b728-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b728-116">Optional request headers</span></span>
| <span data-ttu-id="5b728-117">Имя</span><span class="sxs-lookup"><span data-stu-id="5b728-117">Name</span></span> | <span data-ttu-id="5b728-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5b728-118">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="5b728-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b728-119">Authorization</span></span>  | <span data-ttu-id="5b728-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b728-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b728-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b728-122">Content-Type</span></span>  | <span data-ttu-id="5b728-123">application/json</span><span class="sxs-lookup"><span data-stu-id="5b728-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b728-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b728-124">Request body</span></span>
<span data-ttu-id="5b728-125">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5b728-125">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="5b728-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b728-126">Property</span></span> | <span data-ttu-id="5b728-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5b728-127">Type</span></span> | <span data-ttu-id="5b728-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5b728-128">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5b728-129">values</span><span class="sxs-lookup"><span data-stu-id="5b728-129">values</span></span> | <span data-ttu-id="5b728-130">settingValue</span><span class="sxs-lookup"><span data-stu-id="5b728-130">settingValue</span></span> | <span data-ttu-id="5b728-p103">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="5b728-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="5b728-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b728-134">Response</span></span>

<span data-ttu-id="5b728-135">В случае успешного выполнения этот метод возвращает код отклика `204 OK` и обновленный объект [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b728-135">If successful, this method returns a `204 OK` response code and updated [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b728-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5b728-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b728-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b728-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="5b728-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b728-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->