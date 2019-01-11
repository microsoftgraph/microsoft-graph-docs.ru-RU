---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c303436aafbdbb5167a992f405036b5e00e4d635
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856394"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="7d875-102">Тип ресурса sharingLink</span><span class="sxs-lookup"><span data-stu-id="7d875-102">sharingLink resource type</span></span>

> <span data-ttu-id="7d875-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d875-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d875-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d875-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d875-105">Ресурс **sharingLink** группирует элементы данных, связанных с ссылок в одной структуры.</span><span class="sxs-lookup"><span data-stu-id="7d875-105">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="7d875-106">Если [**разрешение**](permission.md) ресурсов имеет ненулевое **sharingLink** аспекта, разрешение представляет ссылку общего доступа (в отличие от разрешения, предоставленные пользователю или группе).</span><span class="sxs-lookup"><span data-stu-id="7d875-106">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d875-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d875-107">JSON representation</span></span>

<span data-ttu-id="7d875-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d875-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7d875-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d875-109">Properties</span></span>

| <span data-ttu-id="7d875-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d875-110">Property</span></span>       | <span data-ttu-id="7d875-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7d875-111">Type</span></span>          | <span data-ttu-id="7d875-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7d875-112">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="7d875-113">application</span><span class="sxs-lookup"><span data-stu-id="7d875-113">application</span></span>    | <span data-ttu-id="7d875-114">[identity][]</span><span class="sxs-lookup"><span data-stu-id="7d875-114">[identity][]</span></span>  | <span data-ttu-id="7d875-115">Приложение, с которым сопоставлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="7d875-115">The app the link is associated with.</span></span>
| <span data-ttu-id="7d875-116">type</span><span class="sxs-lookup"><span data-stu-id="7d875-116">type</span></span>           | <span data-ttu-id="7d875-117">Строка</span><span class="sxs-lookup"><span data-stu-id="7d875-117">String</span></span>        | <span data-ttu-id="7d875-118">Тип созданной ссылки.</span><span class="sxs-lookup"><span data-stu-id="7d875-118">The type of the link created.</span></span>
| <span data-ttu-id="7d875-119">scope</span><span class="sxs-lookup"><span data-stu-id="7d875-119">scope</span></span>          | <span data-ttu-id="7d875-120">String</span><span class="sxs-lookup"><span data-stu-id="7d875-120">String</span></span>        | <span data-ttu-id="7d875-p102">Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.</span><span class="sxs-lookup"><span data-stu-id="7d875-p102">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="7d875-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="7d875-123">preventsDownload</span></span> | <span data-ttu-id="7d875-124">Логический</span><span class="sxs-lookup"><span data-stu-id="7d875-124">Boolean</span></span>       | <span data-ttu-id="7d875-125">Если значение true, пользователь этой ссылки можно использовать только для просмотра элемента в Интернете и нельзя использовать для загрузки содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="7d875-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="7d875-126">Только для OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d875-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="7d875-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="7d875-127">webHtml</span></span>        | <span data-ttu-id="7d875-128">String</span><span class="sxs-lookup"><span data-stu-id="7d875-128">String</span></span>        | <span data-ttu-id="7d875-129">Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="7d875-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="7d875-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="7d875-130">webUrl</span></span>         | <span data-ttu-id="7d875-131">Строка</span><span class="sxs-lookup"><span data-stu-id="7d875-131">String</span></span>        | <span data-ttu-id="7d875-132">URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7d875-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="7d875-134">Параметры типа</span><span class="sxs-lookup"><span data-stu-id="7d875-134">Type options</span></span>

<span data-ttu-id="7d875-135">Следующая таблица определяет возможные значения для свойства **типа** .</span><span class="sxs-lookup"><span data-stu-id="7d875-135">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="7d875-136">Значение</span><span class="sxs-lookup"><span data-stu-id="7d875-136">Value</span></span>    | <span data-ttu-id="7d875-137">Роль</span><span class="sxs-lookup"><span data-stu-id="7d875-137">Role</span></span>     | <span data-ttu-id="7d875-138">Описание</span><span class="sxs-lookup"><span data-stu-id="7d875-138">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="7d875-139">Ссылка только для просмотра, разрешающая доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d875-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="7d875-140">Ссылка для редактирования, разрешающая доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="7d875-140">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="7d875-141">Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу.</span><span class="sxs-lookup"><span data-stu-id="7d875-141">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="7d875-142">Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d875-142">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="7d875-143">Параметры области</span><span class="sxs-lookup"><span data-stu-id="7d875-143">Scope options</span></span>

<span data-ttu-id="7d875-144">Следующая таблица определяет возможные значения для свойства **области** .</span><span class="sxs-lookup"><span data-stu-id="7d875-144">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="7d875-145">Значение</span><span class="sxs-lookup"><span data-stu-id="7d875-145">Value</span></span>            | <span data-ttu-id="7d875-146">Описание</span><span class="sxs-lookup"><span data-stu-id="7d875-146">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="7d875-147">Лица, имеющие ссылку имеет доступ, без необходимости входа.</span><span class="sxs-lookup"><span data-stu-id="7d875-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="7d875-148">Сюда может входить пользователям за пределами вашей организации.</span><span class="sxs-lookup"><span data-stu-id="7d875-148">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="7d875-149">Любой пользователь вошел в вашей организации (клиента) используйте ссылку для доступа.</span><span class="sxs-lookup"><span data-stu-id="7d875-149">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="7d875-150">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d875-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="7d875-151">Только тех пользователей, которые уже имеют доступ к элементу другими способами возможен доступ к элементу, с помощью этой ссылки.</span><span class="sxs-lookup"><span data-stu-id="7d875-151">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="7d875-152">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d875-152">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="7d875-153">Ссылка предоставляет доступ только к определенному списку людей.</span><span class="sxs-lookup"><span data-stu-id="7d875-153">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="7d875-154">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d875-154">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": ""
}-->
