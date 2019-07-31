---
author: JeremyKelley
description: Ресурс lookupColumn в ресурсе columnDefinition указывает, что значения столбца подставляются из другого источника на сайте.
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8c92bce6b6d7ba401f6b9274f2ba0eee4439929e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009911"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="be3ce-103">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="be3ce-103">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be3ce-104">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="be3ce-104">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be3ce-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="be3ce-105">JSON representation</span></span>

<span data-ttu-id="be3ce-106">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be3ce-106">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="be3ce-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="be3ce-107">Properties</span></span>

| <span data-ttu-id="be3ce-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="be3ce-108">Property name</span></span>             | <span data-ttu-id="be3ce-109">Тип</span><span class="sxs-lookup"><span data-stu-id="be3ce-109">Type</span></span>    | <span data-ttu-id="be3ce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be3ce-110">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="be3ce-111">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="be3ce-111">**allowMultipleValues**</span></span>   | <span data-ttu-id="be3ce-112">boolean</span><span class="sxs-lookup"><span data-stu-id="be3ce-112">boolean</span></span> | <span data-ttu-id="be3ce-113">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="be3ce-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="be3ce-114">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="be3ce-114">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="be3ce-115">boolean</span><span class="sxs-lookup"><span data-stu-id="be3ce-115">boolean</span></span> | <span data-ttu-id="be3ce-116">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="be3ce-116">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="be3ce-117">**columnName**</span><span class="sxs-lookup"><span data-stu-id="be3ce-117">**columnName**</span></span>            | <span data-ttu-id="be3ce-118">string</span><span class="sxs-lookup"><span data-stu-id="be3ce-118">string</span></span>  | <span data-ttu-id="be3ce-119">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="be3ce-119">The name of the lookup source column.</span></span>
| <span data-ttu-id="be3ce-120">**listId**</span><span class="sxs-lookup"><span data-stu-id="be3ce-120">**listId**</span></span>                | <span data-ttu-id="be3ce-121">string</span><span class="sxs-lookup"><span data-stu-id="be3ce-121">string</span></span>  | <span data-ttu-id="be3ce-122">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="be3ce-122">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="be3ce-123">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="be3ce-123">**primaryLookupColumnId**</span></span> | <span data-ttu-id="be3ce-124">string</span><span class="sxs-lookup"><span data-stu-id="be3ce-124">string</span></span>  | <span data-ttu-id="be3ce-125">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="be3ce-125">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="be3ce-126">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="be3ce-126">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

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
