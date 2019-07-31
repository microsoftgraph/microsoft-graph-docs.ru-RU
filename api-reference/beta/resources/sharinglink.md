---
author: JeremyKelley
description: Ресурс sharingLink группирует элементы данных, связанные с ссылками, в единую структуру.
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f1ebff332227410bcb67d87de50a97dd2e078660
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965133"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="a7ad2-103">Тип ресурса sharingLink</span><span class="sxs-lookup"><span data-stu-id="a7ad2-103">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7ad2-104">Ресурс **sharingLink** группирует элементы данных, связанные с ссылками, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-104">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="a7ad2-105">Если ресурс [**Permission**](permission.md) имеет аспект **sharingLink** , отличный от NULL, разрешение представляет ссылку для совместного доступа (в отличие от разрешений, предоставленных пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="a7ad2-105">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7ad2-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7ad2-106">JSON representation</span></span>

<span data-ttu-id="a7ad2-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a7ad2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7ad2-108">Properties</span></span>

| <span data-ttu-id="a7ad2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7ad2-109">Property</span></span>       | <span data-ttu-id="a7ad2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a7ad2-110">Type</span></span>          | <span data-ttu-id="a7ad2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ad2-111">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="a7ad2-112">application</span><span class="sxs-lookup"><span data-stu-id="a7ad2-112">application</span></span>    | <span data-ttu-id="a7ad2-113">[identity][]</span><span class="sxs-lookup"><span data-stu-id="a7ad2-113">[identity][]</span></span>  | <span data-ttu-id="a7ad2-114">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-114">The app the link is associated with.</span></span>
| <span data-ttu-id="a7ad2-115">type</span><span class="sxs-lookup"><span data-stu-id="a7ad2-115">type</span></span>           | <span data-ttu-id="a7ad2-116">String</span><span class="sxs-lookup"><span data-stu-id="a7ad2-116">String</span></span>        | <span data-ttu-id="a7ad2-117">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-117">The type of the link created.</span></span>
| <span data-ttu-id="a7ad2-118">scope</span><span class="sxs-lookup"><span data-stu-id="a7ad2-118">scope</span></span>          | <span data-ttu-id="a7ad2-119">String</span><span class="sxs-lookup"><span data-stu-id="a7ad2-119">String</span></span>        | <span data-ttu-id="a7ad2-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="a7ad2-122">Превентсдовнлоад</span><span class="sxs-lookup"><span data-stu-id="a7ad2-122">preventsDownload</span></span> | <span data-ttu-id="a7ad2-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7ad2-123">Boolean</span></span>       | <span data-ttu-id="a7ad2-124">Если этот параметр имеет значение true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для загрузки содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-124">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="a7ad2-125">Только для OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-125">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="a7ad2-126">webHtml</span><span class="sxs-lookup"><span data-stu-id="a7ad2-126">webHtml</span></span>        | <span data-ttu-id="a7ad2-127">String</span><span class="sxs-lookup"><span data-stu-id="a7ad2-127">String</span></span>        | <span data-ttu-id="a7ad2-128">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-128">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="a7ad2-129">webUrl</span><span class="sxs-lookup"><span data-stu-id="a7ad2-129">webUrl</span></span>         | <span data-ttu-id="a7ad2-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a7ad2-130">String</span></span>        | <span data-ttu-id="a7ad2-131">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-131">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="a7ad2-133">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="a7ad2-133">Type options</span></span>

<span data-ttu-id="a7ad2-134">В приведенной ниже таблице определены возможные значения свойства **Type** .</span><span class="sxs-lookup"><span data-stu-id="a7ad2-134">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="a7ad2-135">Значение</span><span class="sxs-lookup"><span data-stu-id="a7ad2-135">Value</span></span>    | <span data-ttu-id="a7ad2-136">Роль</span><span class="sxs-lookup"><span data-stu-id="a7ad2-136">Role</span></span>     | <span data-ttu-id="a7ad2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ad2-137">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="a7ad2-138">Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-138">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="a7ad2-139">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-139">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="a7ad2-p103">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="a7ad2-142">Параметры области</span><span class="sxs-lookup"><span data-stu-id="a7ad2-142">Scope options</span></span>

<span data-ttu-id="a7ad2-143">В приведенной ниже таблице определены возможные значения для свойства **Scope** .</span><span class="sxs-lookup"><span data-stu-id="a7ad2-143">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="a7ad2-144">Значение</span><span class="sxs-lookup"><span data-stu-id="a7ad2-144">Value</span></span>            | <span data-ttu-id="a7ad2-145">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ad2-145">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="a7ad2-146">Любой пользователь, у которого есть ссылка, имеет доступ, не требуя входа в систему.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="a7ad2-147">Сюда могут относиться пользователи за прев Организации.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-147">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="a7ad2-148">Любой пользователь, вошедший в организацию (клиент), может использовать эту ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="a7ad2-149">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-149">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="a7ad2-150">С помощью этой ссылки можно получить доступ к элементу только пользователям, у которых уже есть доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-150">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="a7ad2-151">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-151">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="a7ad2-152">Эта ссылка предоставляет доступ только к определенному списку пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-152">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="a7ad2-153">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a7ad2-153">Only available in OneDrive for Business and SharePoint.</span></span>

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
