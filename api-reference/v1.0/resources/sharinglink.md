---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: Ресурс SharingLink группирует связанные ссылками элементы данных в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: def93edc26d90d40b480243431316c60a7f34e37
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239809"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="7521a-103">Тип ресурса SharingLink</span><span class="sxs-lookup"><span data-stu-id="7521a-103">SharingLink resource type</span></span>

<span data-ttu-id="7521a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7521a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7521a-105">Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="7521a-105">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="7521a-106">Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="7521a-106">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7521a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7521a-107">JSON representation</span></span>

<span data-ttu-id="7521a-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7521a-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7521a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7521a-109">Properties</span></span>

| <span data-ttu-id="7521a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7521a-110">Property</span></span>    | <span data-ttu-id="7521a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7521a-111">Type</span></span>          | <span data-ttu-id="7521a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7521a-112">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="7521a-113">application</span><span class="sxs-lookup"><span data-stu-id="7521a-113">application</span></span> | <span data-ttu-id="7521a-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="7521a-114">[identity][]</span></span>  | <span data-ttu-id="7521a-115">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="7521a-115">The app the link is associated with.</span></span>
| <span data-ttu-id="7521a-116">type</span><span class="sxs-lookup"><span data-stu-id="7521a-116">type</span></span>        | <span data-ttu-id="7521a-117">String</span><span class="sxs-lookup"><span data-stu-id="7521a-117">String</span></span>        | <span data-ttu-id="7521a-118">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="7521a-118">The type of the link created.</span></span>
| <span data-ttu-id="7521a-119">scope</span><span class="sxs-lookup"><span data-stu-id="7521a-119">scope</span></span>       | <span data-ttu-id="7521a-120">String</span><span class="sxs-lookup"><span data-stu-id="7521a-120">String</span></span>        | <span data-ttu-id="7521a-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="7521a-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="7521a-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="7521a-123">preventsDownload</span></span> | <span data-ttu-id="7521a-124">Логическое</span><span class="sxs-lookup"><span data-stu-id="7521a-124">Boolean</span></span>       | <span data-ttu-id="7521a-125">Если используется true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для скачивания содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="7521a-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="7521a-126">Только для OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7521a-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="7521a-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="7521a-127">webHtml</span></span>     | <span data-ttu-id="7521a-128">String</span><span class="sxs-lookup"><span data-stu-id="7521a-128">String</span></span>        | <span data-ttu-id="7521a-129">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="7521a-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="7521a-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="7521a-130">webUrl</span></span>      | <span data-ttu-id="7521a-131">String</span><span class="sxs-lookup"><span data-stu-id="7521a-131">String</span></span>        | <span data-ttu-id="7521a-132">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7521a-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="7521a-134">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="7521a-134">Type options</span></span>

<span data-ttu-id="7521a-135">В таблице ниже определены возможные значения свойства **type**.</span><span class="sxs-lookup"><span data-stu-id="7521a-135">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="7521a-136">Значение</span><span class="sxs-lookup"><span data-stu-id="7521a-136">Value</span></span>   | <span data-ttu-id="7521a-137">Роль</span><span class="sxs-lookup"><span data-stu-id="7521a-137">Role</span></span>    | <span data-ttu-id="7521a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="7521a-138">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="7521a-139">Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7521a-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="7521a-140">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="7521a-140">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="7521a-p103">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7521a-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="7521a-143">Параметры области</span><span class="sxs-lookup"><span data-stu-id="7521a-143">Scope options</span></span>

| <span data-ttu-id="7521a-144">Значение</span><span class="sxs-lookup"><span data-stu-id="7521a-144">Value</span></span>          | <span data-ttu-id="7521a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="7521a-145">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="7521a-146">Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="7521a-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="7521a-147">Это также относится к людям вне вашей организации.</span><span class="sxs-lookup"><span data-stu-id="7521a-147">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="7521a-148">Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="7521a-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="7521a-149">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7521a-149">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->

