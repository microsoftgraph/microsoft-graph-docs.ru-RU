---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: Контент
localization_priority: Normal
description: Ресурс contentType представляет тип контента в SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c05ed39c0f92b209925fc9a722c5562999ae438c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531780"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="97906-103">Тип ресурса contentType</span><span class="sxs-lookup"><span data-stu-id="97906-103">ContentType resource type</span></span>

<span data-ttu-id="97906-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97906-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97906-105">Ресурс **contentType** представляет _тип контента_ в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97906-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="97906-106">Типы контента позволяют определить набор столбцов, которые должны присутствовать в каждом элементе [**ListItem**][listItem] в [**списке**][list].</span><span class="sxs-lookup"><span data-stu-id="97906-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="97906-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97906-107">JSON representation</span></span>

<span data-ttu-id="97906-108">Ниже показано представление ресурса **contentType** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97906-108">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a><span data-ttu-id="97906-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="97906-109">Properties</span></span>

| <span data-ttu-id="97906-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97906-110">Property name</span></span>     | <span data-ttu-id="97906-111">Тип</span><span class="sxs-lookup"><span data-stu-id="97906-111">Type</span></span>                 | <span data-ttu-id="97906-112">Описание</span><span class="sxs-lookup"><span data-stu-id="97906-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="97906-113">**description**</span><span class="sxs-lookup"><span data-stu-id="97906-113">**description**</span></span>   | <span data-ttu-id="97906-114">строка</span><span class="sxs-lookup"><span data-stu-id="97906-114">string</span></span>               | <span data-ttu-id="97906-115">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="97906-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="97906-116">**group**</span><span class="sxs-lookup"><span data-stu-id="97906-116">**group**</span></span>         | <span data-ttu-id="97906-117">string</span><span class="sxs-lookup"><span data-stu-id="97906-117">string</span></span>               | <span data-ttu-id="97906-118">Имя группы, которой принадлежит этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="97906-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="97906-119">Позволяет упорядочить связанные типы контента.</span><span class="sxs-lookup"><span data-stu-id="97906-119">Helps organize related content types.</span></span>
| <span data-ttu-id="97906-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="97906-120">**hidden**</span></span>        | <span data-ttu-id="97906-121">логический</span><span class="sxs-lookup"><span data-stu-id="97906-121">boolean</span></span>              | <span data-ttu-id="97906-122">Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.</span><span class="sxs-lookup"><span data-stu-id="97906-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="97906-123">**id**</span><span class="sxs-lookup"><span data-stu-id="97906-123">**id**</span></span>            | <span data-ttu-id="97906-124">строка</span><span class="sxs-lookup"><span data-stu-id="97906-124">string</span></span>               | <span data-ttu-id="97906-125">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="97906-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="97906-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="97906-126">**inheritedFrom**</span></span> | <span data-ttu-id="97906-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="97906-127">[itemReference][]</span></span>    | <span data-ttu-id="97906-128">Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.</span><span class="sxs-lookup"><span data-stu-id="97906-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="97906-129">**name**</span><span class="sxs-lookup"><span data-stu-id="97906-129">**name**</span></span>          | <span data-ttu-id="97906-130">string</span><span class="sxs-lookup"><span data-stu-id="97906-130">string</span></span>               | <span data-ttu-id="97906-131">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="97906-131">The name of the content type.</span></span>
| <span data-ttu-id="97906-132">**order**</span><span class="sxs-lookup"><span data-stu-id="97906-132">**order**</span></span>         | <span data-ttu-id="97906-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="97906-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="97906-134">Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="97906-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="97906-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="97906-135">**parentId**</span></span>      | <span data-ttu-id="97906-136">string</span><span class="sxs-lookup"><span data-stu-id="97906-136">string</span></span>               | <span data-ttu-id="97906-137">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="97906-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="97906-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="97906-138">**readOnly**</span></span>      | <span data-ttu-id="97906-139">boolean</span><span class="sxs-lookup"><span data-stu-id="97906-139">boolean</span></span>              | <span data-ttu-id="97906-140">Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.</span><span class="sxs-lookup"><span data-stu-id="97906-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="97906-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="97906-141">**sealed**</span></span>        | <span data-ttu-id="97906-142">boolean</span><span class="sxs-lookup"><span data-stu-id="97906-142">boolean</span></span>              | <span data-ttu-id="97906-143">Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз.</span><span class="sxs-lookup"><span data-stu-id="97906-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="97906-144">Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.</span><span class="sxs-lookup"><span data-stu-id="97906-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="97906-145">Связи</span><span class="sxs-lookup"><span data-stu-id="97906-145">Relationships</span></span>

| <span data-ttu-id="97906-146">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97906-146">Property name</span></span>   | <span data-ttu-id="97906-147">Тип</span><span class="sxs-lookup"><span data-stu-id="97906-147">Type</span></span>                      | <span data-ttu-id="97906-148">Описание</span><span class="sxs-lookup"><span data-stu-id="97906-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="97906-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="97906-149">**columnLinks**</span></span> | <span data-ttu-id="97906-150">Коллекция [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="97906-150">[columnLink][] collection</span></span> | <span data-ttu-id="97906-151">Коллекция столбцов, необходимых для этого типа контента</span><span class="sxs-lookup"><span data-stu-id="97906-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="97906-152">Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="97906-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
