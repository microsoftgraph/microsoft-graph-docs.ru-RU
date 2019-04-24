---
title: Тип ресурса Items
description: Объект item в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507310"
---
# <a name="items-resource-type"></a><span data-ttu-id="27007-103">Тип ресурса Items</span><span class="sxs-lookup"><span data-stu-id="27007-103">items resource type</span></span>
<span data-ttu-id="27007-104">Представляет элемент в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="27007-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="27007-105">Методы</span><span class="sxs-lookup"><span data-stu-id="27007-105">Methods</span></span>

| <span data-ttu-id="27007-106">Метод</span><span class="sxs-lookup"><span data-stu-id="27007-106">Method</span></span>                                      |<span data-ttu-id="27007-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27007-107">Return Type</span></span>|<span data-ttu-id="27007-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27007-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="27007-109">Получение элементов</span><span class="sxs-lookup"><span data-stu-id="27007-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="27007-110">items</span><span class="sxs-lookup"><span data-stu-id="27007-110">items</span></span>     |<span data-ttu-id="27007-111">Возвращает объект Item.</span><span class="sxs-lookup"><span data-stu-id="27007-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="27007-112">Размещение элементов</span><span class="sxs-lookup"><span data-stu-id="27007-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="27007-113">items</span><span class="sxs-lookup"><span data-stu-id="27007-113">items</span></span>     |<span data-ttu-id="27007-114">Создает объект Item.</span><span class="sxs-lookup"><span data-stu-id="27007-114">Creates an item object.</span></span>|
|[<span data-ttu-id="27007-115">Элемент Patch</span><span class="sxs-lookup"><span data-stu-id="27007-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="27007-116">items</span><span class="sxs-lookup"><span data-stu-id="27007-116">items</span></span>     |<span data-ttu-id="27007-117">Обновляет объект Item.</span><span class="sxs-lookup"><span data-stu-id="27007-117">Updates an item object.</span></span>|
|[<span data-ttu-id="27007-118">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="27007-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="27007-119">Нет</span><span class="sxs-lookup"><span data-stu-id="27007-119">none</span></span>      |<span data-ttu-id="27007-120">Удаляет объект Item.</span><span class="sxs-lookup"><span data-stu-id="27007-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27007-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="27007-121">Properties</span></span>
| <span data-ttu-id="27007-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="27007-122">Property</span></span>           | <span data-ttu-id="27007-123">Тип</span><span class="sxs-lookup"><span data-stu-id="27007-123">Type</span></span> |<span data-ttu-id="27007-124">Описание</span><span class="sxs-lookup"><span data-stu-id="27007-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="27007-125">id</span><span class="sxs-lookup"><span data-stu-id="27007-125">id</span></span>                  |<span data-ttu-id="27007-126">GUID</span><span class="sxs-lookup"><span data-stu-id="27007-126">GUID</span></span>    |<span data-ttu-id="27007-127">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-127">The unique ID of the item.</span></span> <span data-ttu-id="27007-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="27007-128">Non-editable.</span></span>             |
|<span data-ttu-id="27007-129">number</span><span class="sxs-lookup"><span data-stu-id="27007-129">number</span></span>              |<span data-ttu-id="27007-130">строка</span><span class="sxs-lookup"><span data-stu-id="27007-130">string</span></span>  |<span data-ttu-id="27007-131">Номер элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-131">The item number.</span></span>                                     |
|<span data-ttu-id="27007-132">displayName</span><span class="sxs-lookup"><span data-stu-id="27007-132">displayName</span></span>         |<span data-ttu-id="27007-133">string</span><span class="sxs-lookup"><span data-stu-id="27007-133">string</span></span>  |<span data-ttu-id="27007-134">Задает описание элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="27007-135">type</span><span class="sxs-lookup"><span data-stu-id="27007-135">type</span></span>                |<span data-ttu-id="27007-136">числовых</span><span class="sxs-lookup"><span data-stu-id="27007-136">numeric</span></span> |<span data-ttu-id="27007-137">Тип запасов для элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-137">The inventory type for the item.</span></span> <span data-ttu-id="27007-138">1 = складская номенклатура, 2 = сервисный товар.</span><span class="sxs-lookup"><span data-stu-id="27007-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="27007-139">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="27007-139">This is a required property.</span></span>|
|<span data-ttu-id="27007-140">заблокированных</span><span class="sxs-lookup"><span data-stu-id="27007-140">blocked</span></span>             |<span data-ttu-id="27007-141">логический</span><span class="sxs-lookup"><span data-stu-id="27007-141">boolean</span></span> |<span data-ttu-id="27007-142">Указывает, что транзакции с элементом не могут быть опубликованы, например, потому что элемент находится в карантине.</span><span class="sxs-lookup"><span data-stu-id="27007-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="27007-143">Имеет значение **true**, если элемент блокируется.</span><span class="sxs-lookup"><span data-stu-id="27007-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="27007-144">Басеунитофмеасуреид</span><span class="sxs-lookup"><span data-stu-id="27007-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="27007-145">GUID</span><span class="sxs-lookup"><span data-stu-id="27007-145">GUID</span></span>    |<span data-ttu-id="27007-146">Задает идентификатор единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="27007-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="27007-147">Басеунитофмеасуре</span><span class="sxs-lookup"><span data-stu-id="27007-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="27007-148">Навигационная. Унитофмеасуре</span><span class="sxs-lookup"><span data-stu-id="27007-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="27007-149">Задает единицу измерения, в которой хранится элемент в перечне.</span><span class="sxs-lookup"><span data-stu-id="27007-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="27007-150">GTIN</span><span class="sxs-lookup"><span data-stu-id="27007-150">gtin</span></span>                |<span data-ttu-id="27007-151">числовых</span><span class="sxs-lookup"><span data-stu-id="27007-151">numeric</span></span> |<span data-ttu-id="27007-152">Это номер глобального торгового элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="27007-153">Итемкатегорид</span><span class="sxs-lookup"><span data-stu-id="27007-153">itemCategoryId</span></span>      |<span data-ttu-id="27007-154">GUID</span><span class="sxs-lookup"><span data-stu-id="27007-154">GUID</span></span> |<span data-ttu-id="27007-155">Указывает категорию, к которой принадлежит элемент.</span><span class="sxs-lookup"><span data-stu-id="27007-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="27007-156">Категории элементов также содержат назначенные атрибуты элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="27007-157">inventory</span><span class="sxs-lookup"><span data-stu-id="27007-157">inventory</span></span>           |<span data-ttu-id="27007-158">числе</span><span class="sxs-lookup"><span data-stu-id="27007-158">decimal</span></span> |<span data-ttu-id="27007-159">Указывает, сколько единиц товара, таких как штуки, коробки или г., находится на складе.</span><span class="sxs-lookup"><span data-stu-id="27007-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="27007-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27007-160">Read-Only.</span></span>|
|<span data-ttu-id="27007-161">unitPrice</span><span class="sxs-lookup"><span data-stu-id="27007-161">unitPrice</span></span>           |<span data-ttu-id="27007-162">числе</span><span class="sxs-lookup"><span data-stu-id="27007-162">decimal</span></span> |<span data-ttu-id="27007-163">Указывает цену для одной единицы элемента в указанной валюте.</span><span class="sxs-lookup"><span data-stu-id="27007-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="27007-164">Прицеинклудестакс</span><span class="sxs-lookup"><span data-stu-id="27007-164">priceIncludesTax</span></span>    |<span data-ttu-id="27007-165">логический</span><span class="sxs-lookup"><span data-stu-id="27007-165">boolean</span></span> |<span data-ttu-id="27007-166">Указывает, что цена включает налог.</span><span class="sxs-lookup"><span data-stu-id="27007-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="27007-167">Имеет значение **true**, если цена включает налог.</span><span class="sxs-lookup"><span data-stu-id="27007-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="27007-168">Униткост</span><span class="sxs-lookup"><span data-stu-id="27007-168">unitCost</span></span>            |<span data-ttu-id="27007-169">числе</span><span class="sxs-lookup"><span data-stu-id="27007-169">decimal</span></span> |<span data-ttu-id="27007-170">Указывает затраты на единицу измерения элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="27007-171">Таксграупид</span><span class="sxs-lookup"><span data-stu-id="27007-171">taxGroupId</span></span>          |<span data-ttu-id="27007-172">GUID</span><span class="sxs-lookup"><span data-stu-id="27007-172">GUID</span></span>    |<span data-ttu-id="27007-173">Указывает идентификатор налоговой группы для элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="27007-174">Таксграупкоде</span><span class="sxs-lookup"><span data-stu-id="27007-174">taxGroupCode</span></span>        |<span data-ttu-id="27007-175">числовых</span><span class="sxs-lookup"><span data-stu-id="27007-175">numeric</span></span> |<span data-ttu-id="27007-176">Группа налогов представляет группу складских элементов или ресурсов, которые могут быть идентичными налоговым условиям.</span><span class="sxs-lookup"><span data-stu-id="27007-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="27007-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27007-177">lastModifiedDateTime</span></span>|<span data-ttu-id="27007-178">отличным</span><span class="sxs-lookup"><span data-stu-id="27007-178">datetime</span></span>|<span data-ttu-id="27007-179">Дата и время последнего изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="27007-179">The last datetime the item was modified.</span></span> <span data-ttu-id="27007-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27007-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="27007-181">Связи</span><span class="sxs-lookup"><span data-stu-id="27007-181">Relationships</span></span>
<span data-ttu-id="27007-182">Налоговая группа (Таксграупкоде) должна существовать в таблице налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="27007-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27007-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27007-183">JSON representation</span></span>

<span data-ttu-id="27007-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27007-184">Here is a JSON representation of the resource.</span></span>


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


