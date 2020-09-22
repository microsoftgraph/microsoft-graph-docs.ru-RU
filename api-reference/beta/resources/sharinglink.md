---
author: JeremyKelley
description: Ресурс sharingLink группирует элементы данных, связанные с ссылками, в единую структуру.
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6c79de95408b334d11dd6c2682dc12a0679f686c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010166"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="01de6-103">Тип ресурса sharingLink</span><span class="sxs-lookup"><span data-stu-id="01de6-103">sharingLink resource type</span></span>

<span data-ttu-id="01de6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01de6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01de6-105">Ресурс **sharingLink** группирует элементы данных, связанные с ссылками, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="01de6-105">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="01de6-106">Если ресурс [**Permission**](permission.md) имеет аспект **sharingLink** , отличный от NULL, разрешение представляет ссылку для совместного доступа (в отличие от разрешений, предоставленных пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="01de6-106">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="01de6-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01de6-107">JSON representation</span></span>

<span data-ttu-id="01de6-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01de6-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="01de6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="01de6-109">Properties</span></span>

| <span data-ttu-id="01de6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="01de6-110">Property</span></span>       | <span data-ttu-id="01de6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="01de6-111">Type</span></span>          | <span data-ttu-id="01de6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="01de6-112">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="01de6-113">application</span><span class="sxs-lookup"><span data-stu-id="01de6-113">application</span></span>    | <span data-ttu-id="01de6-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="01de6-114">[identity][]</span></span>  | <span data-ttu-id="01de6-115">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="01de6-115">The app the link is associated with.</span></span>
| <span data-ttu-id="01de6-116">type</span><span class="sxs-lookup"><span data-stu-id="01de6-116">type</span></span>           | <span data-ttu-id="01de6-117">String</span><span class="sxs-lookup"><span data-stu-id="01de6-117">String</span></span>        | <span data-ttu-id="01de6-118">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="01de6-118">The type of the link created.</span></span>
| <span data-ttu-id="01de6-119">scope</span><span class="sxs-lookup"><span data-stu-id="01de6-119">scope</span></span>          | <span data-ttu-id="01de6-120">String</span><span class="sxs-lookup"><span data-stu-id="01de6-120">String</span></span>        | <span data-ttu-id="01de6-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="01de6-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="01de6-123">превентсдовнлоад</span><span class="sxs-lookup"><span data-stu-id="01de6-123">preventsDownload</span></span> | <span data-ttu-id="01de6-124">Логическое</span><span class="sxs-lookup"><span data-stu-id="01de6-124">Boolean</span></span>       | <span data-ttu-id="01de6-125">Если этот параметр имеет значение true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для загрузки содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="01de6-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="01de6-126">Только для OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01de6-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="01de6-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="01de6-127">webHtml</span></span>        | <span data-ttu-id="01de6-128">String</span><span class="sxs-lookup"><span data-stu-id="01de6-128">String</span></span>        | <span data-ttu-id="01de6-129">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="01de6-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="01de6-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="01de6-130">webUrl</span></span>         | <span data-ttu-id="01de6-131">String</span><span class="sxs-lookup"><span data-stu-id="01de6-131">String</span></span>        | <span data-ttu-id="01de6-132">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="01de6-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="01de6-134">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="01de6-134">Type options</span></span>

<span data-ttu-id="01de6-135">В приведенной ниже таблице определены возможные значения свойства **Type** .</span><span class="sxs-lookup"><span data-stu-id="01de6-135">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="01de6-136">Значение</span><span class="sxs-lookup"><span data-stu-id="01de6-136">Value</span></span>    | <span data-ttu-id="01de6-137">Role</span><span class="sxs-lookup"><span data-stu-id="01de6-137">Role</span></span>     | <span data-ttu-id="01de6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="01de6-138">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="01de6-139">Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01de6-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="01de6-140">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="01de6-140">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="01de6-p103">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01de6-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="01de6-143">Параметры области</span><span class="sxs-lookup"><span data-stu-id="01de6-143">Scope options</span></span>

<span data-ttu-id="01de6-144">В приведенной ниже таблице определены возможные значения для свойства **Scope** .</span><span class="sxs-lookup"><span data-stu-id="01de6-144">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="01de6-145">Значение</span><span class="sxs-lookup"><span data-stu-id="01de6-145">Value</span></span>            | <span data-ttu-id="01de6-146">Описание</span><span class="sxs-lookup"><span data-stu-id="01de6-146">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="01de6-147">Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="01de6-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="01de6-148">Это также относится к людям вне вашей организации.</span><span class="sxs-lookup"><span data-stu-id="01de6-148">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="01de6-149">Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="01de6-149">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="01de6-150">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01de6-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="01de6-151">С помощью этой ссылки можно получить доступ к элементу только пользователям, у которых уже есть доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="01de6-151">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="01de6-152">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01de6-152">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="01de6-153">Эта ссылка предоставляет доступ только к определенному списку пользователей.</span><span class="sxs-lookup"><span data-stu-id="01de6-153">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="01de6-154">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="01de6-154">Only available in OneDrive for Business and SharePoint.</span></span>

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


