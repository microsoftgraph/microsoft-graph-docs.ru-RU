---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 04b9a92bfd723b188fc6869717a5665e10b6af30
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345182"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="a0d22-102">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="a0d22-102">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d22-103">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="a0d22-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0d22-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a0d22-104">JSON representation</span></span>

<span data-ttu-id="a0d22-105">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d22-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="a0d22-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0d22-106">Properties</span></span>

| <span data-ttu-id="a0d22-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a0d22-107">Property name</span></span>             | <span data-ttu-id="a0d22-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a0d22-108">Type</span></span>    | <span data-ttu-id="a0d22-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d22-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="a0d22-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="a0d22-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="a0d22-111">boolean</span><span class="sxs-lookup"><span data-stu-id="a0d22-111">boolean</span></span> | <span data-ttu-id="a0d22-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="a0d22-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a0d22-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="a0d22-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="a0d22-114">boolean</span><span class="sxs-lookup"><span data-stu-id="a0d22-114">boolean</span></span> | <span data-ttu-id="a0d22-115">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="a0d22-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="a0d22-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="a0d22-116">**columnName**</span></span>            | <span data-ttu-id="a0d22-117">string</span><span class="sxs-lookup"><span data-stu-id="a0d22-117">string</span></span>  | <span data-ttu-id="a0d22-118">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="a0d22-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="a0d22-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="a0d22-119">**listId**</span></span>                | <span data-ttu-id="a0d22-120">string</span><span class="sxs-lookup"><span data-stu-id="a0d22-120">string</span></span>  | <span data-ttu-id="a0d22-121">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="a0d22-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="a0d22-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="a0d22-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="a0d22-123">string</span><span class="sxs-lookup"><span data-stu-id="a0d22-123">string</span></span>  | <span data-ttu-id="a0d22-124">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="a0d22-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="a0d22-125">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="a0d22-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

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
