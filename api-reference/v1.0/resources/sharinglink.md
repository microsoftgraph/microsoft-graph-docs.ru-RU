---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: Ресурс SharingLink группирует связанные ссылками элементы данных в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3195207588061840c4e1394e1460f74d3728510c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446865"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="89a36-103">Тип ресурса SharingLink</span><span class="sxs-lookup"><span data-stu-id="89a36-103">SharingLink resource type</span></span>

<span data-ttu-id="89a36-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="89a36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89a36-105">Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="89a36-105">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="89a36-106">Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="89a36-106">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="89a36-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89a36-107">JSON representation</span></span>

<span data-ttu-id="89a36-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89a36-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="89a36-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="89a36-109">Properties</span></span>

| <span data-ttu-id="89a36-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="89a36-110">Property</span></span>    | <span data-ttu-id="89a36-111">Тип</span><span class="sxs-lookup"><span data-stu-id="89a36-111">Type</span></span>          | <span data-ttu-id="89a36-112">Описание</span><span class="sxs-lookup"><span data-stu-id="89a36-112">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="89a36-113">application</span><span class="sxs-lookup"><span data-stu-id="89a36-113">application</span></span> | <span data-ttu-id="89a36-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="89a36-114">[identity][]</span></span>  | <span data-ttu-id="89a36-115">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="89a36-115">The app the link is associated with.</span></span>
| <span data-ttu-id="89a36-116">type</span><span class="sxs-lookup"><span data-stu-id="89a36-116">type</span></span>        | <span data-ttu-id="89a36-117">String</span><span class="sxs-lookup"><span data-stu-id="89a36-117">String</span></span>        | <span data-ttu-id="89a36-118">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="89a36-118">The type of the link created.</span></span>
| <span data-ttu-id="89a36-119">scope</span><span class="sxs-lookup"><span data-stu-id="89a36-119">scope</span></span>       | <span data-ttu-id="89a36-120">String</span><span class="sxs-lookup"><span data-stu-id="89a36-120">String</span></span>        | <span data-ttu-id="89a36-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="89a36-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="89a36-123">webHtml</span><span class="sxs-lookup"><span data-stu-id="89a36-123">webHtml</span></span>     | <span data-ttu-id="89a36-124">String</span><span class="sxs-lookup"><span data-stu-id="89a36-124">String</span></span>        | <span data-ttu-id="89a36-125">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="89a36-125">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="89a36-126">webUrl</span><span class="sxs-lookup"><span data-stu-id="89a36-126">webUrl</span></span>      | <span data-ttu-id="89a36-127">Строка</span><span class="sxs-lookup"><span data-stu-id="89a36-127">String</span></span>        | <span data-ttu-id="89a36-128">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="89a36-128">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="89a36-130">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="89a36-130">Type options</span></span>

<span data-ttu-id="89a36-131">В таблице ниже определены возможные значения свойства **type**.</span><span class="sxs-lookup"><span data-stu-id="89a36-131">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="89a36-132">Значение</span><span class="sxs-lookup"><span data-stu-id="89a36-132">Value</span></span>   | <span data-ttu-id="89a36-133">Роль</span><span class="sxs-lookup"><span data-stu-id="89a36-133">Role</span></span>    | <span data-ttu-id="89a36-134">Описание</span><span class="sxs-lookup"><span data-stu-id="89a36-134">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="89a36-135">Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89a36-135">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="89a36-136">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="89a36-136">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="89a36-p102">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="89a36-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="89a36-139">Параметры области</span><span class="sxs-lookup"><span data-stu-id="89a36-139">Scope options</span></span>

| <span data-ttu-id="89a36-140">Значение</span><span class="sxs-lookup"><span data-stu-id="89a36-140">Value</span></span>          | <span data-ttu-id="89a36-141">Описание</span><span class="sxs-lookup"><span data-stu-id="89a36-141">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="89a36-142">Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="89a36-142">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="89a36-143">Это также относится к людям вне вашей организации.</span><span class="sxs-lookup"><span data-stu-id="89a36-143">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="89a36-144">Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="89a36-144">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="89a36-145">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="89a36-145">Only available in OneDrive for Business and SharePoint.</span></span>

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
