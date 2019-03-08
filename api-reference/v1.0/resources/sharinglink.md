---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: f16f8240800be4b9c1780a4057583381b736f079
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481428"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="86aa6-102">Тип ресурса SharingLink</span><span class="sxs-lookup"><span data-stu-id="86aa6-102">SharingLink resource type</span></span>

<span data-ttu-id="86aa6-103">Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="86aa6-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="86aa6-104">Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="86aa6-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="86aa6-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86aa6-105">JSON representation</span></span>

<span data-ttu-id="86aa6-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86aa6-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="86aa6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86aa6-107">Properties</span></span>

| <span data-ttu-id="86aa6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86aa6-108">Property</span></span>    | <span data-ttu-id="86aa6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86aa6-109">Type</span></span>          | <span data-ttu-id="86aa6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86aa6-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="86aa6-111">application</span><span class="sxs-lookup"><span data-stu-id="86aa6-111">application</span></span> | <span data-ttu-id="86aa6-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="86aa6-112">[identity][]</span></span>  | <span data-ttu-id="86aa6-113">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="86aa6-113">The app the link is associated with.</span></span>
| <span data-ttu-id="86aa6-114">type</span><span class="sxs-lookup"><span data-stu-id="86aa6-114">type</span></span>        | <span data-ttu-id="86aa6-115">String</span><span class="sxs-lookup"><span data-stu-id="86aa6-115">String</span></span>        | <span data-ttu-id="86aa6-116">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="86aa6-116">The type of the link created.</span></span>
| <span data-ttu-id="86aa6-117">scope</span><span class="sxs-lookup"><span data-stu-id="86aa6-117">scope</span></span>       | <span data-ttu-id="86aa6-118">String</span><span class="sxs-lookup"><span data-stu-id="86aa6-118">String</span></span>        | <span data-ttu-id="86aa6-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="86aa6-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="86aa6-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="86aa6-121">webHtml</span></span>     | <span data-ttu-id="86aa6-122">String</span><span class="sxs-lookup"><span data-stu-id="86aa6-122">String</span></span>        | <span data-ttu-id="86aa6-123">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="86aa6-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="86aa6-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="86aa6-124">webUrl</span></span>      | <span data-ttu-id="86aa6-125">Строка</span><span class="sxs-lookup"><span data-stu-id="86aa6-125">String</span></span>        | <span data-ttu-id="86aa6-126">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="86aa6-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="86aa6-128">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="86aa6-128">Type options</span></span>

<span data-ttu-id="86aa6-129">В таблице ниже определены возможные значения свойства **type**.</span><span class="sxs-lookup"><span data-stu-id="86aa6-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="86aa6-130">Значение</span><span class="sxs-lookup"><span data-stu-id="86aa6-130">Value</span></span>   | <span data-ttu-id="86aa6-131">Роль</span><span class="sxs-lookup"><span data-stu-id="86aa6-131">Role</span></span>    | <span data-ttu-id="86aa6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86aa6-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="86aa6-133">Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86aa6-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="86aa6-134">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="86aa6-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="86aa6-p102">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="86aa6-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="86aa6-137">Параметры области</span><span class="sxs-lookup"><span data-stu-id="86aa6-137">Scope options</span></span>

| <span data-ttu-id="86aa6-138">Значение</span><span class="sxs-lookup"><span data-stu-id="86aa6-138">Value</span></span>          | <span data-ttu-id="86aa6-139">Описание</span><span class="sxs-lookup"><span data-stu-id="86aa6-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="86aa6-140">Любой пользователь, у которого есть ссылка, имеет доступ, не требуя входа в систему.</span><span class="sxs-lookup"><span data-stu-id="86aa6-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="86aa6-141">Сюда могут относиться пользователи за прев Организации.</span><span class="sxs-lookup"><span data-stu-id="86aa6-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="86aa6-142">Любой пользователь, вошедший в организацию (клиент), может использовать эту ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="86aa6-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="86aa6-143">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="86aa6-143">Only available in OneDrive for Business and SharePoint.</span></span>

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
