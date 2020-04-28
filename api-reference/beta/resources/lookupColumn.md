---
author: JeremyKelley
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 813b31b61e3f510107cdd27ed64ec44fba9d0550
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522892"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="c550e-103">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="c550e-103">LookupColumn resource type</span></span>

<span data-ttu-id="c550e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c550e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c550e-105">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="c550e-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c550e-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c550e-106">JSON representation</span></span>

<span data-ttu-id="c550e-107">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c550e-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c550e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c550e-108">Properties</span></span>

| <span data-ttu-id="c550e-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c550e-109">Property name</span></span>             | <span data-ttu-id="c550e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c550e-110">Type</span></span>    | <span data-ttu-id="c550e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c550e-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="c550e-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="c550e-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="c550e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="c550e-113">boolean</span></span> | <span data-ttu-id="c550e-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="c550e-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="c550e-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="c550e-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="c550e-116">boolean</span><span class="sxs-lookup"><span data-stu-id="c550e-116">boolean</span></span> | <span data-ttu-id="c550e-117">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="c550e-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="c550e-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="c550e-118">**columnName**</span></span>            | <span data-ttu-id="c550e-119">string</span><span class="sxs-lookup"><span data-stu-id="c550e-119">string</span></span>  | <span data-ttu-id="c550e-120">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="c550e-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="c550e-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="c550e-121">**listId**</span></span>                | <span data-ttu-id="c550e-122">string</span><span class="sxs-lookup"><span data-stu-id="c550e-122">string</span></span>  | <span data-ttu-id="c550e-123">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="c550e-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="c550e-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="c550e-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="c550e-125">string</span><span class="sxs-lookup"><span data-stu-id="c550e-125">string</span></span>  | <span data-ttu-id="c550e-126">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="c550e-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="c550e-127">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="c550e-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->
