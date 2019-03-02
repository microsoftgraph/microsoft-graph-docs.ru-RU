---
title: Тип ресурса Items
description: Объект item в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365964"
---
# <a name="items-resource-type"></a><span data-ttu-id="8a791-103">Тип ресурса Items</span><span class="sxs-lookup"><span data-stu-id="8a791-103">items resource type</span></span>
<span data-ttu-id="8a791-104">Представляет элемент в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="8a791-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8a791-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8a791-105">Methods</span></span>

| <span data-ttu-id="8a791-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8a791-106">Method</span></span>                                      |<span data-ttu-id="8a791-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a791-107">Return Type</span></span>|<span data-ttu-id="8a791-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8a791-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="8a791-109">Получение элементов</span><span class="sxs-lookup"><span data-stu-id="8a791-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="8a791-110">items</span><span class="sxs-lookup"><span data-stu-id="8a791-110">items</span></span>     |<span data-ttu-id="8a791-111">Возвращает объект Item.</span><span class="sxs-lookup"><span data-stu-id="8a791-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="8a791-112">Размещение элементов</span><span class="sxs-lookup"><span data-stu-id="8a791-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="8a791-113">items</span><span class="sxs-lookup"><span data-stu-id="8a791-113">items</span></span>     |<span data-ttu-id="8a791-114">Создает объект Item.</span><span class="sxs-lookup"><span data-stu-id="8a791-114">Creates an item object.</span></span>|
|[<span data-ttu-id="8a791-115">Элемент Patch</span><span class="sxs-lookup"><span data-stu-id="8a791-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="8a791-116">items</span><span class="sxs-lookup"><span data-stu-id="8a791-116">items</span></span>     |<span data-ttu-id="8a791-117">Обновляет объект Item.</span><span class="sxs-lookup"><span data-stu-id="8a791-117">Updates an item object.</span></span>|
|[<span data-ttu-id="8a791-118">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="8a791-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="8a791-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8a791-119">none</span></span>      |<span data-ttu-id="8a791-120">Удаляет объект Item.</span><span class="sxs-lookup"><span data-stu-id="8a791-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a791-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a791-121">Properties</span></span>
| <span data-ttu-id="8a791-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a791-122">Property</span></span>           | <span data-ttu-id="8a791-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8a791-123">Type</span></span> |<span data-ttu-id="8a791-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8a791-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="8a791-125">id</span><span class="sxs-lookup"><span data-stu-id="8a791-125">id</span></span>                  |<span data-ttu-id="8a791-126">GUID</span><span class="sxs-lookup"><span data-stu-id="8a791-126">GUID</span></span>    |<span data-ttu-id="8a791-127">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-127">The unique ID of the item.</span></span> <span data-ttu-id="8a791-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="8a791-128">Non-editable.</span></span>             |
|<span data-ttu-id="8a791-129">number</span><span class="sxs-lookup"><span data-stu-id="8a791-129">number</span></span>              |<span data-ttu-id="8a791-130">строка</span><span class="sxs-lookup"><span data-stu-id="8a791-130">string</span></span>  |<span data-ttu-id="8a791-131">Номер элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-131">The item number.</span></span>                                     |
|<span data-ttu-id="8a791-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8a791-132">displayName</span></span>         |<span data-ttu-id="8a791-133">строка</span><span class="sxs-lookup"><span data-stu-id="8a791-133">string</span></span>  |<span data-ttu-id="8a791-134">Задает описание элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="8a791-135">type</span><span class="sxs-lookup"><span data-stu-id="8a791-135">type</span></span>                |<span data-ttu-id="8a791-136">числовых</span><span class="sxs-lookup"><span data-stu-id="8a791-136">numeric</span></span> |<span data-ttu-id="8a791-137">Тип запасов для элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-137">The inventory type for the item.</span></span> <span data-ttu-id="8a791-138">1 = складская номенклатура, 2 = сервисный товар.</span><span class="sxs-lookup"><span data-stu-id="8a791-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="8a791-139">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8a791-139">This is a required property.</span></span>|
|<span data-ttu-id="8a791-140">заблокировано</span><span class="sxs-lookup"><span data-stu-id="8a791-140">blocked</span></span>             |<span data-ttu-id="8a791-141">boolean</span><span class="sxs-lookup"><span data-stu-id="8a791-141">boolean</span></span> |<span data-ttu-id="8a791-142">Указывает, что транзакции с элементом не могут быть опубликованы, например, потому что элемент находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="8a791-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="8a791-143">Имеет значение **true**, если элемент блокируется.</span><span class="sxs-lookup"><span data-stu-id="8a791-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="8a791-144">Басеунитофмеасуреид</span><span class="sxs-lookup"><span data-stu-id="8a791-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="8a791-145">GUID</span><span class="sxs-lookup"><span data-stu-id="8a791-145">GUID</span></span>    |<span data-ttu-id="8a791-146">Задает идентификатор единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="8a791-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="8a791-147">Басеунитофмеасуре</span><span class="sxs-lookup"><span data-stu-id="8a791-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="8a791-148">Навигационная. Унитофмеасуре</span><span class="sxs-lookup"><span data-stu-id="8a791-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="8a791-149">Задает единицу измерения, в которой хранится элемент в перечне.</span><span class="sxs-lookup"><span data-stu-id="8a791-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="8a791-150">GTIN</span><span class="sxs-lookup"><span data-stu-id="8a791-150">gtin</span></span>                |<span data-ttu-id="8a791-151">числовых</span><span class="sxs-lookup"><span data-stu-id="8a791-151">numeric</span></span> |<span data-ttu-id="8a791-152">Это номер глобального торгового элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="8a791-153">Итемкатегорид</span><span class="sxs-lookup"><span data-stu-id="8a791-153">itemCategoryId</span></span>      |<span data-ttu-id="8a791-154">GUID</span><span class="sxs-lookup"><span data-stu-id="8a791-154">GUID</span></span> |<span data-ttu-id="8a791-155">Указывает категорию, к которой принадлежит элемент.</span><span class="sxs-lookup"><span data-stu-id="8a791-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="8a791-156">Категории элементов также содержат назначенные атрибуты элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="8a791-157">inventory</span><span class="sxs-lookup"><span data-stu-id="8a791-157">inventory</span></span>           |<span data-ttu-id="8a791-158">числе</span><span class="sxs-lookup"><span data-stu-id="8a791-158">decimal</span></span> |<span data-ttu-id="8a791-159">Указывает, сколько единиц товара, таких как штуки, коробки или г., находится на складе.</span><span class="sxs-lookup"><span data-stu-id="8a791-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="8a791-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a791-160">Read-Only.</span></span>|
|<span data-ttu-id="8a791-161">unitPrice</span><span class="sxs-lookup"><span data-stu-id="8a791-161">unitPrice</span></span>           |<span data-ttu-id="8a791-162">числе</span><span class="sxs-lookup"><span data-stu-id="8a791-162">decimal</span></span> |<span data-ttu-id="8a791-163">Указывает цену для одной единицы элемента в указанной валюте.</span><span class="sxs-lookup"><span data-stu-id="8a791-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="8a791-164">Прицеинклудестакс</span><span class="sxs-lookup"><span data-stu-id="8a791-164">priceIncludesTax</span></span>    |<span data-ttu-id="8a791-165">boolean</span><span class="sxs-lookup"><span data-stu-id="8a791-165">boolean</span></span> |<span data-ttu-id="8a791-166">Указывает, что цена включает налог.</span><span class="sxs-lookup"><span data-stu-id="8a791-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="8a791-167">Имеет значение **true**, если цена включает налог.</span><span class="sxs-lookup"><span data-stu-id="8a791-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="8a791-168">Униткост</span><span class="sxs-lookup"><span data-stu-id="8a791-168">unitCost</span></span>            |<span data-ttu-id="8a791-169">числе</span><span class="sxs-lookup"><span data-stu-id="8a791-169">decimal</span></span> |<span data-ttu-id="8a791-170">Указывает затраты на единицу измерения элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="8a791-171">Таксграупид</span><span class="sxs-lookup"><span data-stu-id="8a791-171">taxGroupId</span></span>          |<span data-ttu-id="8a791-172">GUID</span><span class="sxs-lookup"><span data-stu-id="8a791-172">GUID</span></span>    |<span data-ttu-id="8a791-173">Указывает идентификатор налоговой группы для элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="8a791-174">Таксграупкоде</span><span class="sxs-lookup"><span data-stu-id="8a791-174">taxGroupCode</span></span>        |<span data-ttu-id="8a791-175">числовых</span><span class="sxs-lookup"><span data-stu-id="8a791-175">numeric</span></span> |<span data-ttu-id="8a791-176">Группа налогов представляет группу складских элементов или ресурсов, которые могут быть идентичными налоговым условиям.</span><span class="sxs-lookup"><span data-stu-id="8a791-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="8a791-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a791-177">lastModifiedDateTime</span></span>|<span data-ttu-id="8a791-178">отличным</span><span class="sxs-lookup"><span data-stu-id="8a791-178">datetime</span></span>|<span data-ttu-id="8a791-179">Дата и время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="8a791-179">The last datetime the item was modified.</span></span> <span data-ttu-id="8a791-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a791-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="8a791-181">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a791-181">Relationships</span></span>
<span data-ttu-id="8a791-182">Налоговая группа (Таксграупкоде) должна существовать в таблице налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8a791-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a791-183">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8a791-183">JSON representation</span></span>

<span data-ttu-id="8a791-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a791-184">Here is a JSON representation of the resource.</span></span>


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


