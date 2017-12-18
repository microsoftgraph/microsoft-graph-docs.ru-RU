# <a name="update-a-group-setting"></a><span data-ttu-id="07d7b-101">Обновление параметра группы</span><span class="sxs-lookup"><span data-stu-id="07d7b-101">Update a group setting</span></span>

<span data-ttu-id="07d7b-102">Обновление свойств для указанных объектов параметров группы.</span><span class="sxs-lookup"><span data-stu-id="07d7b-102">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="07d7b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07d7b-103">Permissions</span></span>

<span data-ttu-id="07d7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="07d7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="07d7b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07d7b-106">Permission type</span></span>      | <span data-ttu-id="07d7b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07d7b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d7b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07d7b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="07d7b-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07d7b-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07d7b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07d7b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d7b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d7b-111">Not supported.</span></span>    |
|<span data-ttu-id="07d7b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07d7b-112">Application</span></span> | <span data-ttu-id="07d7b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d7b-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07d7b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07d7b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="07d7b-115">Обновление параметра на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="07d7b-115">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="07d7b-116">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07d7b-116">Optional request headers</span></span>
| <span data-ttu-id="07d7b-117">Имя</span><span class="sxs-lookup"><span data-stu-id="07d7b-117">Name</span></span> | <span data-ttu-id="07d7b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="07d7b-118">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="07d7b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07d7b-119">Authorization</span></span>  | <span data-ttu-id="07d7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07d7b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07d7b-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07d7b-122">Content-Type</span></span>  | <span data-ttu-id="07d7b-123">application/json</span><span class="sxs-lookup"><span data-stu-id="07d7b-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07d7b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07d7b-124">Request body</span></span>
<span data-ttu-id="07d7b-125">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="07d7b-125">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="07d7b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="07d7b-126">Property</span></span> | <span data-ttu-id="07d7b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="07d7b-127">Type</span></span> | <span data-ttu-id="07d7b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="07d7b-128">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="07d7b-129">values</span><span class="sxs-lookup"><span data-stu-id="07d7b-129">values</span></span> | <span data-ttu-id="07d7b-130">settingValue</span><span class="sxs-lookup"><span data-stu-id="07d7b-130">settingValue</span></span> | <span data-ttu-id="07d7b-p103">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="07d7b-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="07d7b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d7b-134">Response</span></span>

<span data-ttu-id="07d7b-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07d7b-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07d7b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="07d7b-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="07d7b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d7b-137">Request</span></span>
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
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "True"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="07d7b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d7b-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
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
