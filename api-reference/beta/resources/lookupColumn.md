---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: lookupColumn
localization_priority: Normal
ms.openlocfilehash: 1c7ab364777e1e3f82bb78d8e0940cf4f85576a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885710"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="98916-102">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="98916-102">LookupColumn resource type</span></span>

> <span data-ttu-id="98916-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98916-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98916-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98916-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98916-105">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="98916-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98916-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98916-106">JSON representation</span></span>

<span data-ttu-id="98916-107">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98916-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="98916-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98916-108">Properties</span></span>

| <span data-ttu-id="98916-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="98916-109">Property name</span></span>             | <span data-ttu-id="98916-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98916-110">Type</span></span>    | <span data-ttu-id="98916-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98916-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="98916-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="98916-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="98916-113">логический</span><span class="sxs-lookup"><span data-stu-id="98916-113">boolean</span></span> | <span data-ttu-id="98916-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="98916-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="98916-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="98916-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="98916-116">логический</span><span class="sxs-lookup"><span data-stu-id="98916-116">boolean</span></span> | <span data-ttu-id="98916-117">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="98916-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="98916-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="98916-118">**columnName**</span></span>            | <span data-ttu-id="98916-119">строка</span><span class="sxs-lookup"><span data-stu-id="98916-119">string</span></span>  | <span data-ttu-id="98916-120">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="98916-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="98916-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="98916-121">**listId**</span></span>                | <span data-ttu-id="98916-122">строка</span><span class="sxs-lookup"><span data-stu-id="98916-122">string</span></span>  | <span data-ttu-id="98916-123">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="98916-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="98916-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="98916-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="98916-125">строка</span><span class="sxs-lookup"><span data-stu-id="98916-125">string</span></span>  | <span data-ttu-id="98916-126">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="98916-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="98916-127">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="98916-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
