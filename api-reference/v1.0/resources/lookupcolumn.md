---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 752d60bbb1ac93b5a58eb326e7a6769921c47a66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447523"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="eb887-103">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="eb887-103">LookupColumn resource type</span></span>

<span data-ttu-id="eb887-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb887-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb887-105">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="eb887-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb887-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="eb887-106">JSON representation</span></span>

<span data-ttu-id="eb887-107">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb887-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="eb887-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb887-108">Properties</span></span>

| <span data-ttu-id="eb887-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="eb887-109">Property name</span></span>             | <span data-ttu-id="eb887-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb887-110">Type</span></span>    | <span data-ttu-id="eb887-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb887-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="eb887-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="eb887-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="eb887-113">boolean</span><span class="sxs-lookup"><span data-stu-id="eb887-113">boolean</span></span> | <span data-ttu-id="eb887-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="eb887-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="eb887-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="eb887-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="eb887-116">boolean</span><span class="sxs-lookup"><span data-stu-id="eb887-116">boolean</span></span> | <span data-ttu-id="eb887-117">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="eb887-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="eb887-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="eb887-118">**columnName**</span></span>            | <span data-ttu-id="eb887-119">string</span><span class="sxs-lookup"><span data-stu-id="eb887-119">string</span></span>  | <span data-ttu-id="eb887-120">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="eb887-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="eb887-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="eb887-121">**listId**</span></span>                | <span data-ttu-id="eb887-122">string</span><span class="sxs-lookup"><span data-stu-id="eb887-122">string</span></span>  | <span data-ttu-id="eb887-123">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="eb887-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="eb887-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="eb887-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="eb887-125">string</span><span class="sxs-lookup"><span data-stu-id="eb887-125">string</span></span>  | <span data-ttu-id="eb887-126">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="eb887-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="eb887-127">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="eb887-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
