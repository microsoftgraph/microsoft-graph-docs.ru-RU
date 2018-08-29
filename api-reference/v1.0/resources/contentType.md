---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentType
ms.openlocfilehash: cb16559aa9da3a885be1977bbd1466265d0a72f0
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268335"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="beb56-102">Тип ресурса contentType</span><span class="sxs-lookup"><span data-stu-id="beb56-102">ContentType resource type</span></span>

<span data-ttu-id="beb56-103">Ресурс **contentType** представляет _тип контента_ в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="beb56-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="beb56-104">Типы контента позволяют задать набор столбцов, которые должны присутствовать в каждом элементе [**listItem**][listItem] в [**списке**][list].</span><span class="sxs-lookup"><span data-stu-id="beb56-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listItem.md

## <a name="json-representation"></a><span data-ttu-id="beb56-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="beb56-105">JSON representation</span></span>

<span data-ttu-id="beb56-106">Ниже показано представление ресурса **contentType** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beb56-106">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="beb56-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="beb56-107">Properties</span></span>

| <span data-ttu-id="beb56-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="beb56-108">Property name</span></span>     | <span data-ttu-id="beb56-109">Тип</span><span class="sxs-lookup"><span data-stu-id="beb56-109">Type</span></span>                 | <span data-ttu-id="beb56-110">Описание</span><span class="sxs-lookup"><span data-stu-id="beb56-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="beb56-111">**description**</span><span class="sxs-lookup"><span data-stu-id="beb56-111">**description**</span></span>   | <span data-ttu-id="beb56-112">строка</span><span class="sxs-lookup"><span data-stu-id="beb56-112">string</span></span>               | <span data-ttu-id="beb56-113">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="beb56-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="beb56-114">**group**</span><span class="sxs-lookup"><span data-stu-id="beb56-114">**group**</span></span>         | <span data-ttu-id="beb56-115">строка</span><span class="sxs-lookup"><span data-stu-id="beb56-115">string</span></span>               | <span data-ttu-id="beb56-116">Имя группы, которой принадлежит этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="beb56-117">Позволяет упорядочить связанные типы контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-117">Helps organize related content types.</span></span>
| <span data-ttu-id="beb56-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="beb56-118">**hidden**</span></span>        | <span data-ttu-id="beb56-119">логический</span><span class="sxs-lookup"><span data-stu-id="beb56-119">boolean</span></span>              | <span data-ttu-id="beb56-120">Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.</span><span class="sxs-lookup"><span data-stu-id="beb56-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="beb56-121">**id**</span><span class="sxs-lookup"><span data-stu-id="beb56-121">**id**</span></span>            | <span data-ttu-id="beb56-122">строка</span><span class="sxs-lookup"><span data-stu-id="beb56-122">string</span></span>               | <span data-ttu-id="beb56-123">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="beb56-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="beb56-124">**inheritedFrom**</span></span> | <span data-ttu-id="beb56-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="beb56-125">[itemReference][]</span></span>    | <span data-ttu-id="beb56-126">Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="beb56-127">**name**</span><span class="sxs-lookup"><span data-stu-id="beb56-127">**name**</span></span>          | <span data-ttu-id="beb56-128">строка</span><span class="sxs-lookup"><span data-stu-id="beb56-128">string</span></span>               | <span data-ttu-id="beb56-129">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-129">The name of the content type.</span></span>
| <span data-ttu-id="beb56-130">**order**</span><span class="sxs-lookup"><span data-stu-id="beb56-130">**order**</span></span>         | <span data-ttu-id="beb56-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="beb56-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="beb56-132">Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="beb56-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="beb56-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="beb56-133">**parentId**</span></span>      | <span data-ttu-id="beb56-134">строка</span><span class="sxs-lookup"><span data-stu-id="beb56-134">string</span></span>               | <span data-ttu-id="beb56-135">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="beb56-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="beb56-136">**readOnly**</span></span>      | <span data-ttu-id="beb56-137">логический</span><span class="sxs-lookup"><span data-stu-id="beb56-137">boolean</span></span>              | <span data-ttu-id="beb56-138">Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.</span><span class="sxs-lookup"><span data-stu-id="beb56-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="beb56-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="beb56-139">**sealed**</span></span>        | <span data-ttu-id="beb56-140">логический</span><span class="sxs-lookup"><span data-stu-id="beb56-140">boolean</span></span>              | <span data-ttu-id="beb56-141">Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз.</span><span class="sxs-lookup"><span data-stu-id="beb56-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="beb56-142">Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.</span><span class="sxs-lookup"><span data-stu-id="beb56-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="beb56-143">Связи</span><span class="sxs-lookup"><span data-stu-id="beb56-143">Relationships</span></span>

| <span data-ttu-id="beb56-144">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="beb56-144">Property name</span></span>   | <span data-ttu-id="beb56-145">Тип</span><span class="sxs-lookup"><span data-stu-id="beb56-145">Type</span></span>                      | <span data-ttu-id="beb56-146">Описание</span><span class="sxs-lookup"><span data-stu-id="beb56-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="beb56-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="beb56-147">**columnLinks**</span></span> | <span data-ttu-id="beb56-148">Коллекция [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="beb56-148">[columnLink][] collection</span></span> | <span data-ttu-id="beb56-149">Коллекция столбцов, необходимых для этого типа контента</span><span class="sxs-lookup"><span data-stu-id="beb56-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="beb56-150">Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="beb56-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
