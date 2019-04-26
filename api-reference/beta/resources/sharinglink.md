---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c5a08ca3a1a7b91d5cd2277a71f1301adf5edc93
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343101"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="a5629-102">Тип ресурса sharingLink</span><span class="sxs-lookup"><span data-stu-id="a5629-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5629-103">Ресурс **sharingLink** группирует элементы данных, связанные с ссылками, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="a5629-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="a5629-104">Если ресурс [**Permission**](permission.md) имеет аспект **sharingLink** , отличный от NULL, разрешение представляет ссылку для совместного доступа (в отличие от разрешений, предоставленных пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="a5629-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5629-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5629-105">JSON representation</span></span>

<span data-ttu-id="a5629-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5629-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a5629-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5629-107">Properties</span></span>

| <span data-ttu-id="a5629-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5629-108">Property</span></span>       | <span data-ttu-id="a5629-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5629-109">Type</span></span>          | <span data-ttu-id="a5629-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5629-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="a5629-111">application</span><span class="sxs-lookup"><span data-stu-id="a5629-111">application</span></span>    | <span data-ttu-id="a5629-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="a5629-112">[identity][]</span></span>  | <span data-ttu-id="a5629-113">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="a5629-113">The app the link is associated with.</span></span>
| <span data-ttu-id="a5629-114">type</span><span class="sxs-lookup"><span data-stu-id="a5629-114">type</span></span>           | <span data-ttu-id="a5629-115">String</span><span class="sxs-lookup"><span data-stu-id="a5629-115">String</span></span>        | <span data-ttu-id="a5629-116">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="a5629-116">The type of the link created.</span></span>
| <span data-ttu-id="a5629-117">scope</span><span class="sxs-lookup"><span data-stu-id="a5629-117">scope</span></span>          | <span data-ttu-id="a5629-118">String</span><span class="sxs-lookup"><span data-stu-id="a5629-118">String</span></span>        | <span data-ttu-id="a5629-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="a5629-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="a5629-121">Превентсдовнлоад</span><span class="sxs-lookup"><span data-stu-id="a5629-121">preventsDownload</span></span> | <span data-ttu-id="a5629-122">Логический</span><span class="sxs-lookup"><span data-stu-id="a5629-122">Boolean</span></span>       | <span data-ttu-id="a5629-123">Если этот параметр имеет значение true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для загрузки содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5629-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="a5629-124">Только для OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5629-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="a5629-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="a5629-125">webHtml</span></span>        | <span data-ttu-id="a5629-126">String</span><span class="sxs-lookup"><span data-stu-id="a5629-126">String</span></span>        | <span data-ttu-id="a5629-127">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="a5629-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="a5629-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="a5629-128">webUrl</span></span>         | <span data-ttu-id="a5629-129">Строка</span><span class="sxs-lookup"><span data-stu-id="a5629-129">String</span></span>        | <span data-ttu-id="a5629-130">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a5629-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="a5629-132">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="a5629-132">Type options</span></span>

<span data-ttu-id="a5629-133">В приведенной ниже таблице определены возможные значения свойства **Type** .</span><span class="sxs-lookup"><span data-stu-id="a5629-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="a5629-134">Значение</span><span class="sxs-lookup"><span data-stu-id="a5629-134">Value</span></span>    | <span data-ttu-id="a5629-135">Роль</span><span class="sxs-lookup"><span data-stu-id="a5629-135">Role</span></span>     | <span data-ttu-id="a5629-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a5629-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="a5629-137">Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5629-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="a5629-138">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="a5629-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="a5629-p103">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5629-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="a5629-141">Параметры области</span><span class="sxs-lookup"><span data-stu-id="a5629-141">Scope options</span></span>

<span data-ttu-id="a5629-142">В приведенной ниже таблице определены возможные значения для свойства **Scope** .</span><span class="sxs-lookup"><span data-stu-id="a5629-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="a5629-143">Значение</span><span class="sxs-lookup"><span data-stu-id="a5629-143">Value</span></span>            | <span data-ttu-id="a5629-144">Описание</span><span class="sxs-lookup"><span data-stu-id="a5629-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="a5629-145">Любой пользователь, у которого есть ссылка, имеет доступ, не требуя входа в систему.</span><span class="sxs-lookup"><span data-stu-id="a5629-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="a5629-146">Сюда могут относиться пользователи за прев Организации.</span><span class="sxs-lookup"><span data-stu-id="a5629-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="a5629-147">Любой пользователь, вошедший в организацию (клиент), может использовать эту ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="a5629-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="a5629-148">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5629-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="a5629-149">С помощью этой ссылки можно получить доступ к элементу только пользователям, у которых уже есть доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="a5629-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="a5629-150">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5629-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="a5629-151">Эта ссылка предоставляет доступ только к определенному списку пользователей.</span><span class="sxs-lookup"><span data-stu-id="a5629-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="a5629-152">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5629-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
