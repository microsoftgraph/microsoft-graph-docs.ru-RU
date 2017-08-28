# <a name="sharinglink-resource-type"></a><span data-ttu-id="432bc-101">Тип ресурса SharingLink</span><span class="sxs-lookup"><span data-stu-id="432bc-101">SharingLink resource type</span></span>

<span data-ttu-id="432bc-102">Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="432bc-102">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="432bc-103">Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="432bc-103">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="432bc-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="432bc-104">JSON representation</span></span>

<span data-ttu-id="432bc-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="432bc-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="432bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="432bc-106">Properties</span></span>

| <span data-ttu-id="432bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="432bc-107">Property</span></span>    | <span data-ttu-id="432bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="432bc-108">Type</span></span>                    | <span data-ttu-id="432bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="432bc-109">Description</span></span>                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="432bc-110">application</span><span class="sxs-lookup"><span data-stu-id="432bc-110">application</span></span> | [<span data-ttu-id="432bc-111">identity</span><span class="sxs-lookup"><span data-stu-id="432bc-111">identity</span></span>](identity.md) | <span data-ttu-id="432bc-112">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="432bc-112">The app the link is associated with.</span></span>                                                                                                                                                                    |
| <span data-ttu-id="432bc-113">type</span><span class="sxs-lookup"><span data-stu-id="432bc-113">type</span></span>        | <span data-ttu-id="432bc-114">Строка</span><span class="sxs-lookup"><span data-stu-id="432bc-114">String</span></span>                  | <span data-ttu-id="432bc-115">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="432bc-115">The type of the link created.</span></span>                                                                                                                                                                           |
| <span data-ttu-id="432bc-116">scope</span><span class="sxs-lookup"><span data-stu-id="432bc-116">scope</span></span>       | <span data-ttu-id="432bc-117">String</span><span class="sxs-lookup"><span data-stu-id="432bc-117">String</span></span>                  | <span data-ttu-id="432bc-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="432bc-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span> |
| <span data-ttu-id="432bc-120">webUrl</span><span class="sxs-lookup"><span data-stu-id="432bc-120">webUrl</span></span>      | <span data-ttu-id="432bc-121">Строка</span><span class="sxs-lookup"><span data-stu-id="432bc-121">String</span></span>                  | <span data-ttu-id="432bc-122">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="432bc-122">A URL that opens the item in the browser on the OneDrive website.</span></span>                                                                                                                                       |

## <a name="type-enumeration"></a><span data-ttu-id="432bc-123">Перечисление type</span><span class="sxs-lookup"><span data-stu-id="432bc-123">Type enumeration</span></span>

<span data-ttu-id="432bc-124">В таблице ниже определены возможные значения свойства **type**.</span><span class="sxs-lookup"><span data-stu-id="432bc-124">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="432bc-125">Значение</span><span class="sxs-lookup"><span data-stu-id="432bc-125">Value</span></span>   | <span data-ttu-id="432bc-126">Роль</span><span class="sxs-lookup"><span data-stu-id="432bc-126">Role</span></span>    | <span data-ttu-id="432bc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="432bc-127">Description</span></span>                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | <span data-ttu-id="432bc-128">Ссылка только для просмотра, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="432bc-128">A view-only sharing link, allowing read-only access.</span></span>                            |
| `edit`  | `write` | <span data-ttu-id="432bc-129">Ссылка для совместного доступа на редактирование, разрешающая доступ на чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="432bc-129">An edit sharing link, allowing read-write access.</span></span>                               |

## <a name="scope-enumeration"></a><span data-ttu-id="432bc-130">Перечисление scope</span><span class="sxs-lookup"><span data-stu-id="432bc-130">Scope enumeration</span></span>

| <span data-ttu-id="432bc-131">Значение</span><span class="sxs-lookup"><span data-stu-id="432bc-131">Value</span></span>          | <span data-ttu-id="432bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="432bc-132">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="432bc-133">Ссылку для общего доступа могут использовать все пользователи.</span><span class="sxs-lookup"><span data-stu-id="432bc-133">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="432bc-p102">Ссылку для совместного доступа могут использовать все пользователи в одной и той же организации (клиенте). Эта функция недоступна в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="432bc-p102">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
