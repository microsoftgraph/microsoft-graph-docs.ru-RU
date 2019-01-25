---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521455"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="a5718-102">Тип ресурса SharingLink</span><span class="sxs-lookup"><span data-stu-id="a5718-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5718-103">Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="a5718-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="a5718-104">Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="a5718-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5718-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5718-105">JSON representation</span></span>

<span data-ttu-id="a5718-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5718-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="a5718-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5718-107">Properties</span></span>

| <span data-ttu-id="a5718-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5718-108">Property</span></span>       | <span data-ttu-id="a5718-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5718-109">Type</span></span>          | <span data-ttu-id="a5718-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5718-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="a5718-111">application</span><span class="sxs-lookup"><span data-stu-id="a5718-111">application</span></span>    | <span data-ttu-id="a5718-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="a5718-112">[identity][]</span></span>  | <span data-ttu-id="a5718-113">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="a5718-113">The app the link is associated with.</span></span>
| <span data-ttu-id="a5718-114">type</span><span class="sxs-lookup"><span data-stu-id="a5718-114">type</span></span>           | <span data-ttu-id="a5718-115">Строка</span><span class="sxs-lookup"><span data-stu-id="a5718-115">String</span></span>        | <span data-ttu-id="a5718-116">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="a5718-116">The type of the link created.</span></span>
| <span data-ttu-id="a5718-117">scope</span><span class="sxs-lookup"><span data-stu-id="a5718-117">scope</span></span>          | <span data-ttu-id="a5718-118">String</span><span class="sxs-lookup"><span data-stu-id="a5718-118">String</span></span>        | <span data-ttu-id="a5718-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="a5718-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="a5718-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="a5718-121">preventsDownload</span></span> | <span data-ttu-id="a5718-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="a5718-122">Boolean</span></span>       | <span data-ttu-id="a5718-123">Если значение true, пользователь этой ссылки можно использовать только для просмотра элемента в Интернете и нельзя использовать для загрузки содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5718-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="a5718-124">Только для OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5718-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="a5718-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="a5718-125">webHtml</span></span>        | <span data-ttu-id="a5718-126">String</span><span class="sxs-lookup"><span data-stu-id="a5718-126">String</span></span>        | <span data-ttu-id="a5718-127">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="a5718-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="a5718-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="a5718-128">webUrl</span></span>         | <span data-ttu-id="a5718-129">Строка</span><span class="sxs-lookup"><span data-stu-id="a5718-129">String</span></span>        | <span data-ttu-id="a5718-130">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a5718-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="a5718-132">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="a5718-132">Type options</span></span>

<span data-ttu-id="a5718-133">Следующая таблица определяет возможные значения для свойства **типа** .</span><span class="sxs-lookup"><span data-stu-id="a5718-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="a5718-134">Значение</span><span class="sxs-lookup"><span data-stu-id="a5718-134">Value</span></span>    | <span data-ttu-id="a5718-135">Роль</span><span class="sxs-lookup"><span data-stu-id="a5718-135">Role</span></span>     | <span data-ttu-id="a5718-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a5718-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="a5718-137">Ссылка только для просмотра, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5718-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="a5718-138">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="a5718-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="a5718-139">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="a5718-139">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="a5718-140">Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5718-140">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="a5718-141">Параметры области</span><span class="sxs-lookup"><span data-stu-id="a5718-141">Scope options</span></span>

<span data-ttu-id="a5718-142">Следующая таблица определяет возможные значения для свойства **области** .</span><span class="sxs-lookup"><span data-stu-id="a5718-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="a5718-143">Значение</span><span class="sxs-lookup"><span data-stu-id="a5718-143">Value</span></span>            | <span data-ttu-id="a5718-144">Описание</span><span class="sxs-lookup"><span data-stu-id="a5718-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="a5718-145">Лица, имеющие ссылку имеет доступ, без необходимости входа.</span><span class="sxs-lookup"><span data-stu-id="a5718-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="a5718-146">Сюда может входить пользователям за пределами вашей организации.</span><span class="sxs-lookup"><span data-stu-id="a5718-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="a5718-147">Любой пользователь вошел в вашей организации (клиента) используйте ссылку для доступа.</span><span class="sxs-lookup"><span data-stu-id="a5718-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="a5718-148">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5718-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="a5718-149">Только тех пользователей, которые уже имеют доступ к элементу другими способами возможен доступ к элементу, с помощью этой ссылки.</span><span class="sxs-lookup"><span data-stu-id="a5718-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="a5718-150">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5718-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="a5718-151">Ссылка предоставляет доступ только к определенному списку людей.</span><span class="sxs-lookup"><span data-stu-id="a5718-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="a5718-152">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5718-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
