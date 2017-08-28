# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="5e9d5-101">Создание ссылки для совместного доступа для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="5e9d5-101">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="5e9d5-102">Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-102">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="5e9d5-p101">Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="5e9d5-105">Ресурсы DriveItem наследуют разрешения от своих предков.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-105">DriveItem resources inherit permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e9d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e9d5-106">Permissions</span></span>
<span data-ttu-id="5e9d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5e9d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e9d5-109">Permission type</span></span>      | <span data-ttu-id="5e9d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e9d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e9d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e9d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e9d5-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e9d5-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e9d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e9d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e9d5-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e9d5-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e9d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e9d5-115">Application</span></span> | <span data-ttu-id="5e9d5-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e9d5-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e9d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e9d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a><span data-ttu-id="5e9d5-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e9d5-118">Request body</span></span>
<span data-ttu-id="5e9d5-p103">В теле запроса определяется тип ссылки для совместного доступа, нужной приложению. Запрос должен содержать объект JSON с указанным ниже свойством.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p103">The body of the request defines the type of sharing link your application is looking for. The request should be a JSON object with this property.</span></span>

| <span data-ttu-id="5e9d5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5e9d5-121">Name</span></span>      | <span data-ttu-id="5e9d5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5e9d5-122">Type</span></span>   | <span data-ttu-id="5e9d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5e9d5-123">Description</span></span>                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| <span data-ttu-id="5e9d5-124">**type**</span><span class="sxs-lookup"><span data-stu-id="5e9d5-124">**type**</span></span>  | <span data-ttu-id="5e9d5-125">string</span><span class="sxs-lookup"><span data-stu-id="5e9d5-125">string</span></span> | <span data-ttu-id="5e9d5-p104">Тип создаваемой ссылки для совместного доступа. Возможные значения: `view`, `edit` или `embed`.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="5e9d5-128">**scope**</span><span class="sxs-lookup"><span data-stu-id="5e9d5-128">**scope**</span></span> | <span data-ttu-id="5e9d5-129">string</span><span class="sxs-lookup"><span data-stu-id="5e9d5-129">string</span></span> | <span data-ttu-id="5e9d5-p105">Область создаваемой ссылки. Возможные значения: `anonymous` или `organization`. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p105">The scope of link to create. Either `anonymous` or `organization`. Optional.</span></span> |

## <a name="link-types"></a><span data-ttu-id="5e9d5-133">Типы ссылок</span><span class="sxs-lookup"><span data-stu-id="5e9d5-133">Link types</span></span>
<span data-ttu-id="5e9d5-134">Параметр **type** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-134">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="5e9d5-135">Значение типа</span><span class="sxs-lookup"><span data-stu-id="5e9d5-135">Type value</span></span> | <span data-ttu-id="5e9d5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="5e9d5-136">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="5e9d5-137">Создает ссылку на элемент, предполагающую доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-137">Creates a read-only link to the item.</span></span>                                                        |
| `edit`     | <span data-ttu-id="5e9d5-138">Создает ссылку на элемент, предполагающую доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-138">Creates a read-write link to the item.</span></span>                                                       |
| `embed`    | <span data-ttu-id="5e9d5-p106">Создает встроенную ссылку на элемент. Этот вариант доступен только для личных учетных записей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p106">Creates an embeddable link to the item. This option is only available for OneDrive Personal.</span></span> |

## <a name="scope-types"></a><span data-ttu-id="5e9d5-141">Типы областей</span><span class="sxs-lookup"><span data-stu-id="5e9d5-141">Scope types</span></span>
<span data-ttu-id="5e9d5-p107">Параметр **scope** может принимать указанные ниже значения. Это необязательный параметр. Если параметр **scope** не указан, создается ссылка с максимальными доступными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p107">The following values are allowed for the **scope** parameter. This is an optional parameter. If the **scope** parameter is not specified, the most permissive link available will be created.</span></span>

| <span data-ttu-id="5e9d5-145">Значение типа</span><span class="sxs-lookup"><span data-stu-id="5e9d5-145">Type value</span></span>     | <span data-ttu-id="5e9d5-146">Описание</span><span class="sxs-lookup"><span data-stu-id="5e9d5-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="5e9d5-p108">Создает доступную всем ссылку на элемент. Администратор клиента может отключить ссылки, не требующие проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p108">Creates a link to the item accessible to anyone. Anonymous links may be disabled by the tenant administrator.</span></span>                 |
| `organization` | <span data-ttu-id="5e9d5-p109">Создает ссылку на элемент, доступную в организации. Область организации для ссылок недоступна в случае личных учетных записей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p109">Creates a link to the item accessible within an organization. Organization link scope is not available for OneDrive Personal.</span></span> |

## <a name="response"></a><span data-ttu-id="5e9d5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e9d5-151">Response</span></span>

<span data-ttu-id="5e9d5-152">В случае успеха этот метод возвращает в теле отклика один ресурс [Permission](../resources/permission.md), представляющий запрашиваемое разрешение для ссылки совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing link permission.</span></span>

<span data-ttu-id="5e9d5-153">Для начала служба проверяет текущие разрешения на наличие значения **type**, подходящего для приложения, совершающего вызов.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-153">The service will first look at the current permissions and check if one already exists that has the same **type** for the calling application.</span></span>

<span data-ttu-id="5e9d5-154">Если для элемента создается новая ссылка совместного доступа, возвращается код отклика `201 Created`, а если возвращается существующая ссылка — код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-154">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="5e9d5-155">Пример</span><span class="sxs-lookup"><span data-stu-id="5e9d5-155">Example</span></span>
<span data-ttu-id="5e9d5-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-156">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5e9d5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e9d5-157">Request</span></span>
<span data-ttu-id="5e9d5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a><span data-ttu-id="5e9d5-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e9d5-159">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="5e9d5-160">Создание ссылок с возможностью общего доступа в компании</span><span class="sxs-lookup"><span data-stu-id="5e9d5-160">Creating company sharable links</span></span>

<span data-ttu-id="5e9d5-p110">OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании. Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующего клиента. Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p110">OneDrive for Business and SharePoint support company sharable links. These are similar to anonymous links, except they only work for members of the owning tenant. To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

## <a name="http-request"></a><span data-ttu-id="5e9d5-164">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e9d5-164">HTTP request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a><span data-ttu-id="5e9d5-165">HTTP-ответ</span><span class="sxs-lookup"><span data-stu-id="5e9d5-165">HTTP response</span></span>

<span data-ttu-id="5e9d5-166">Если для элемента создается новая ссылка для общего доступа, возвращается код ответа `201 Created`, а если возвращается существующая ссылка — код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a><span data-ttu-id="5e9d5-167">Встроенные ссылки</span><span class="sxs-lookup"><span data-stu-id="5e9d5-167">Embeddable links</span></span>

<span data-ttu-id="5e9d5-p111">При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-p111">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="5e9d5-170">**Примечание.** Встроенные ссылки поддерживаются только в ресурсах [Drive](../resources/drive.md), в которых для свойства **driveType** задано значение `personal`.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-170">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <a name="remarks"></a><span data-ttu-id="5e9d5-171">Заметки</span><span class="sxs-lookup"><span data-stu-id="5e9d5-171">Remarks</span></span>

* <span data-ttu-id="5e9d5-172">Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-172">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="5e9d5-173">Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.</span><span class="sxs-lookup"><span data-stu-id="5e9d5-173">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="5e9d5-174">Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).</span><span class="sxs-lookup"><span data-stu-id="5e9d5-174">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
