---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: lookupColumn
ms.openlocfilehash: 07dba3c223ffc3993be1fc284572810a7aa3ccf8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="fecaa-102">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="fecaa-102">LookupColumn resource type</span></span>

<span data-ttu-id="fecaa-103">Ресурс **lookupColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="fecaa-103">The **lookupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fecaa-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fecaa-104">JSON representation</span></span>

<span data-ttu-id="fecaa-105">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fecaa-105">Here is a JSON representation of a **drive** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="fecaa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fecaa-106">Properties</span></span>

| <span data-ttu-id="fecaa-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="fecaa-107">Property name</span></span>             | <span data-ttu-id="fecaa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fecaa-108">Type</span></span>    | <span data-ttu-id="fecaa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fecaa-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="fecaa-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="fecaa-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="fecaa-111">логический</span><span class="sxs-lookup"><span data-stu-id="fecaa-111">boolean</span></span> | <span data-ttu-id="fecaa-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="fecaa-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="fecaa-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="fecaa-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="fecaa-114">логический</span><span class="sxs-lookup"><span data-stu-id="fecaa-114">boolean</span></span> | <span data-ttu-id="fecaa-115">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="fecaa-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="fecaa-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="fecaa-116">**columnName**</span></span>            | <span data-ttu-id="fecaa-117">строка</span><span class="sxs-lookup"><span data-stu-id="fecaa-117">string</span></span>  | <span data-ttu-id="fecaa-118">Имя столбца-источника для подстановки.</span><span class="sxs-lookup"><span data-stu-id="fecaa-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="fecaa-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="fecaa-119">**listId**</span></span>                | <span data-ttu-id="fecaa-120">строка</span><span class="sxs-lookup"><span data-stu-id="fecaa-120">string</span></span>  | <span data-ttu-id="fecaa-121">Уникальный идентификатор списка-источника для подстановки.</span><span class="sxs-lookup"><span data-stu-id="fecaa-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="fecaa-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="fecaa-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="fecaa-123">строка</span><span class="sxs-lookup"><span data-stu-id="fecaa-123">string</span></span>  | <span data-ttu-id="fecaa-124">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="fecaa-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="fecaa-125">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="fecaa-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
