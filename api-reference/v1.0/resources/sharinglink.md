---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="6a6b5-102">Тип ресурса SharingLink</span><span class="sxs-lookup"><span data-stu-id="6a6b5-102">SharingLink resource type</span></span>

<span data-ttu-id="6a6b5-103">Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="6a6b5-104">Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="6a6b5-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a6b5-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a6b5-105">JSON representation</span></span>

<span data-ttu-id="6a6b5-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6a6b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a6b5-107">Properties</span></span>

| <span data-ttu-id="6a6b5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a6b5-108">Property</span></span>    | <span data-ttu-id="6a6b5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6b5-109">Type</span></span>          | <span data-ttu-id="6a6b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6b5-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="6a6b5-111">application</span><span class="sxs-lookup"><span data-stu-id="6a6b5-111">application</span></span> | <span data-ttu-id="6a6b5-112">[identity][]</span><span class="sxs-lookup"><span data-stu-id="6a6b5-112">[identity][]</span></span>  | <span data-ttu-id="6a6b5-113">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-113">The app the link is associated with.</span></span>
| <span data-ttu-id="6a6b5-114">type</span><span class="sxs-lookup"><span data-stu-id="6a6b5-114">type</span></span>        | <span data-ttu-id="6a6b5-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6a6b5-115">String</span></span>        | <span data-ttu-id="6a6b5-116">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-116">The type of the link created.</span></span>
| <span data-ttu-id="6a6b5-117">scope</span><span class="sxs-lookup"><span data-stu-id="6a6b5-117">scope</span></span>       | <span data-ttu-id="6a6b5-118">String</span><span class="sxs-lookup"><span data-stu-id="6a6b5-118">String</span></span>        | <span data-ttu-id="6a6b5-p101">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="6a6b5-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="6a6b5-121">webHtml</span></span>     | <span data-ttu-id="6a6b5-122">String</span><span class="sxs-lookup"><span data-stu-id="6a6b5-122">String</span></span>        | <span data-ttu-id="6a6b5-123">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-123">For embeddable links, this property contains the HTML code for an  element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="6a6b5-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="6a6b5-124">webUrl</span></span>      | <span data-ttu-id="6a6b5-125">Строка</span><span class="sxs-lookup"><span data-stu-id="6a6b5-125">String</span></span>        | <span data-ttu-id="6a6b5-126">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-enumeration"></a><span data-ttu-id="6a6b5-128">Перечисление type</span><span class="sxs-lookup"><span data-stu-id="6a6b5-128">Type enumeration</span></span>

<span data-ttu-id="6a6b5-129">В таблице ниже определены возможные значения свойства **type**.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="6a6b5-130">Значение</span><span class="sxs-lookup"><span data-stu-id="6a6b5-130">Value</span></span>   | <span data-ttu-id="6a6b5-131">Роль</span><span class="sxs-lookup"><span data-stu-id="6a6b5-131">Role</span></span>    | <span data-ttu-id="6a6b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6b5-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="6a6b5-133">Ссылка только для просмотра, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="6a6b5-134">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="6a6b5-135">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="6a6b5-136">Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-enumeration"></a><span data-ttu-id="6a6b5-137">Перечисление областей</span><span class="sxs-lookup"><span data-stu-id="6a6b5-137">Scope enumeration</span></span>

| <span data-ttu-id="6a6b5-138">Значение</span><span class="sxs-lookup"><span data-stu-id="6a6b5-138">Value</span></span>          | <span data-ttu-id="6a6b5-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6b5-139">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="6a6b5-140">Ссылку для общего доступа могут использовать все пользователи.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-140">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="6a6b5-p103">Ссылку для совместного доступа могут использовать все пользователи в одной и той же организации (клиенте). Эта функция недоступна в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-p103">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
