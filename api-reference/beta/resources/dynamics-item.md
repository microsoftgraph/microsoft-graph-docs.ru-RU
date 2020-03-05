---
title: Тип ресурса Items
description: Объект item в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e5578cc2bc05aedd417230cc3e9d3b171e9ba577
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503903"
---
# <a name="items-resource-type"></a><span data-ttu-id="65e2c-103">Тип ресурса Items</span><span class="sxs-lookup"><span data-stu-id="65e2c-103">items resource type</span></span>

<span data-ttu-id="65e2c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65e2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65e2c-105">Представляет элемент в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="65e2c-105">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="65e2c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="65e2c-106">Methods</span></span>

| <span data-ttu-id="65e2c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="65e2c-107">Method</span></span>                                      |<span data-ttu-id="65e2c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65e2c-108">Return Type</span></span>|<span data-ttu-id="65e2c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="65e2c-109">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="65e2c-110">Получение элементов</span><span class="sxs-lookup"><span data-stu-id="65e2c-110">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="65e2c-111">items</span><span class="sxs-lookup"><span data-stu-id="65e2c-111">items</span></span>     |<span data-ttu-id="65e2c-112">Возвращает объект Item.</span><span class="sxs-lookup"><span data-stu-id="65e2c-112">Gets an item object.</span></span>   |
|[<span data-ttu-id="65e2c-113">Размещение элементов</span><span class="sxs-lookup"><span data-stu-id="65e2c-113">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="65e2c-114">items</span><span class="sxs-lookup"><span data-stu-id="65e2c-114">items</span></span>     |<span data-ttu-id="65e2c-115">Создает объект Item.</span><span class="sxs-lookup"><span data-stu-id="65e2c-115">Creates an item object.</span></span>|
|[<span data-ttu-id="65e2c-116">Элемент Patch</span><span class="sxs-lookup"><span data-stu-id="65e2c-116">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="65e2c-117">items</span><span class="sxs-lookup"><span data-stu-id="65e2c-117">items</span></span>     |<span data-ttu-id="65e2c-118">Обновляет объект Item.</span><span class="sxs-lookup"><span data-stu-id="65e2c-118">Updates an item object.</span></span>|
|[<span data-ttu-id="65e2c-119">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="65e2c-119">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="65e2c-120">нет</span><span class="sxs-lookup"><span data-stu-id="65e2c-120">none</span></span>      |<span data-ttu-id="65e2c-121">Удаляет объект Item.</span><span class="sxs-lookup"><span data-stu-id="65e2c-121">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65e2c-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="65e2c-122">Properties</span></span>
| <span data-ttu-id="65e2c-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="65e2c-123">Property</span></span>           | <span data-ttu-id="65e2c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="65e2c-124">Type</span></span> |<span data-ttu-id="65e2c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="65e2c-125">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="65e2c-126">id</span><span class="sxs-lookup"><span data-stu-id="65e2c-126">id</span></span>                  |<span data-ttu-id="65e2c-127">GUID</span><span class="sxs-lookup"><span data-stu-id="65e2c-127">GUID</span></span>    |<span data-ttu-id="65e2c-128">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-128">The unique ID of the item.</span></span> <span data-ttu-id="65e2c-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="65e2c-129">Non-editable.</span></span>             |
|<span data-ttu-id="65e2c-130">число</span><span class="sxs-lookup"><span data-stu-id="65e2c-130">number</span></span>              |<span data-ttu-id="65e2c-131">строка</span><span class="sxs-lookup"><span data-stu-id="65e2c-131">string</span></span>  |<span data-ttu-id="65e2c-132">Номер элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-132">The item number.</span></span>                                     |
|<span data-ttu-id="65e2c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="65e2c-133">displayName</span></span>         |<span data-ttu-id="65e2c-134">string</span><span class="sxs-lookup"><span data-stu-id="65e2c-134">string</span></span>  |<span data-ttu-id="65e2c-135">Задает описание элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-135">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="65e2c-136">type</span><span class="sxs-lookup"><span data-stu-id="65e2c-136">type</span></span>                |<span data-ttu-id="65e2c-137">числовых</span><span class="sxs-lookup"><span data-stu-id="65e2c-137">numeric</span></span> |<span data-ttu-id="65e2c-138">Тип запасов для элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-138">The inventory type for the item.</span></span> <span data-ttu-id="65e2c-139">1 = складская номенклатура, 2 = сервисный товар.</span><span class="sxs-lookup"><span data-stu-id="65e2c-139">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="65e2c-140">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65e2c-140">This is a required property.</span></span>|
|<span data-ttu-id="65e2c-141">заблокированных</span><span class="sxs-lookup"><span data-stu-id="65e2c-141">blocked</span></span>             |<span data-ttu-id="65e2c-142">boolean</span><span class="sxs-lookup"><span data-stu-id="65e2c-142">boolean</span></span> |<span data-ttu-id="65e2c-143">Указывает, что транзакции с элементом не могут быть опубликованы, например, потому что элемент находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="65e2c-143">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="65e2c-144">Имеет значение **true**, если элемент блокируется.</span><span class="sxs-lookup"><span data-stu-id="65e2c-144">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="65e2c-145">басеунитофмеасуреид</span><span class="sxs-lookup"><span data-stu-id="65e2c-145">baseUnitOfMeasureId</span></span> |<span data-ttu-id="65e2c-146">GUID</span><span class="sxs-lookup"><span data-stu-id="65e2c-146">GUID</span></span>    |<span data-ttu-id="65e2c-147">Задает идентификатор единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="65e2c-147">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="65e2c-148">басеунитофмеасуре</span><span class="sxs-lookup"><span data-stu-id="65e2c-148">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="65e2c-149">Навигационная. унитофмеасуре</span><span class="sxs-lookup"><span data-stu-id="65e2c-149">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="65e2c-150">Задает единицу измерения, в которой хранится элемент в перечне.</span><span class="sxs-lookup"><span data-stu-id="65e2c-150">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="65e2c-151">GTIN</span><span class="sxs-lookup"><span data-stu-id="65e2c-151">gtin</span></span>                |<span data-ttu-id="65e2c-152">числовых</span><span class="sxs-lookup"><span data-stu-id="65e2c-152">numeric</span></span> |<span data-ttu-id="65e2c-153">Это номер глобального торгового элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-153">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="65e2c-154">итемкатегорид</span><span class="sxs-lookup"><span data-stu-id="65e2c-154">itemCategoryId</span></span>      |<span data-ttu-id="65e2c-155">GUID</span><span class="sxs-lookup"><span data-stu-id="65e2c-155">GUID</span></span> |<span data-ttu-id="65e2c-156">Указывает категорию, к которой принадлежит элемент.</span><span class="sxs-lookup"><span data-stu-id="65e2c-156">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="65e2c-157">Категории элементов также содержат назначенные атрибуты элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-157">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="65e2c-158">inventory</span><span class="sxs-lookup"><span data-stu-id="65e2c-158">inventory</span></span>           |<span data-ttu-id="65e2c-159">числе</span><span class="sxs-lookup"><span data-stu-id="65e2c-159">decimal</span></span> |<span data-ttu-id="65e2c-160">Указывает, сколько единиц товара, таких как штуки, коробки или г., находится на складе.</span><span class="sxs-lookup"><span data-stu-id="65e2c-160">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="65e2c-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65e2c-161">Read-Only.</span></span>|
|<span data-ttu-id="65e2c-162">unitPrice</span><span class="sxs-lookup"><span data-stu-id="65e2c-162">unitPrice</span></span>           |<span data-ttu-id="65e2c-163">числе</span><span class="sxs-lookup"><span data-stu-id="65e2c-163">decimal</span></span> |<span data-ttu-id="65e2c-164">Указывает цену для одной единицы элемента в указанной валюте.</span><span class="sxs-lookup"><span data-stu-id="65e2c-164">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="65e2c-165">прицеинклудестакс</span><span class="sxs-lookup"><span data-stu-id="65e2c-165">priceIncludesTax</span></span>    |<span data-ttu-id="65e2c-166">boolean</span><span class="sxs-lookup"><span data-stu-id="65e2c-166">boolean</span></span> |<span data-ttu-id="65e2c-167">Указывает, что цена включает налог.</span><span class="sxs-lookup"><span data-stu-id="65e2c-167">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="65e2c-168">Имеет значение **true**, если цена включает налог.</span><span class="sxs-lookup"><span data-stu-id="65e2c-168">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="65e2c-169">униткост</span><span class="sxs-lookup"><span data-stu-id="65e2c-169">unitCost</span></span>            |<span data-ttu-id="65e2c-170">числе</span><span class="sxs-lookup"><span data-stu-id="65e2c-170">decimal</span></span> |<span data-ttu-id="65e2c-171">Указывает затраты на единицу измерения элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-171">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="65e2c-172">таксграупид</span><span class="sxs-lookup"><span data-stu-id="65e2c-172">taxGroupId</span></span>          |<span data-ttu-id="65e2c-173">GUID</span><span class="sxs-lookup"><span data-stu-id="65e2c-173">GUID</span></span>    |<span data-ttu-id="65e2c-174">Указывает идентификатор налоговой группы для элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-174">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="65e2c-175">таксграупкоде</span><span class="sxs-lookup"><span data-stu-id="65e2c-175">taxGroupCode</span></span>        |<span data-ttu-id="65e2c-176">числовых</span><span class="sxs-lookup"><span data-stu-id="65e2c-176">numeric</span></span> |<span data-ttu-id="65e2c-177">Группа налогов представляет группу складских элементов или ресурсов, которые могут быть идентичными налоговым условиям.</span><span class="sxs-lookup"><span data-stu-id="65e2c-177">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="65e2c-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65e2c-178">lastModifiedDateTime</span></span>|<span data-ttu-id="65e2c-179">datetime</span><span class="sxs-lookup"><span data-stu-id="65e2c-179">datetime</span></span>|<span data-ttu-id="65e2c-180">Дата и время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="65e2c-180">The last datetime the item was modified.</span></span> <span data-ttu-id="65e2c-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65e2c-181">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="65e2c-182">Связи</span><span class="sxs-lookup"><span data-stu-id="65e2c-182">Relationships</span></span>
<span data-ttu-id="65e2c-183">Налоговая группа (Таксграупкоде) должна существовать в таблице налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="65e2c-183">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65e2c-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65e2c-184">JSON representation</span></span>

<span data-ttu-id="65e2c-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65e2c-185">Here is a JSON representation of the resource.</span></span>


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


