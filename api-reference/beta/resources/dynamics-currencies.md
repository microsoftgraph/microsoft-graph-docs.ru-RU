---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 42dc5fec859aff758b2f46812a63b10f49f0498a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071369"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="db912-103">Тип ресурса "валюты"</span><span class="sxs-lookup"><span data-stu-id="db912-103">currencies resource type</span></span>

<span data-ttu-id="db912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db912-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db912-105">Представляет валюту, используемую в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="db912-105">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="db912-106">Методы</span><span class="sxs-lookup"><span data-stu-id="db912-106">Methods</span></span>
| <span data-ttu-id="db912-107">Метод</span><span class="sxs-lookup"><span data-stu-id="db912-107">Method</span></span>                                                  |<span data-ttu-id="db912-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db912-108">Return Type</span></span>|<span data-ttu-id="db912-109">Описание</span><span class="sxs-lookup"><span data-stu-id="db912-109">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="db912-110">Получение валют</span><span class="sxs-lookup"><span data-stu-id="db912-110">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="db912-111">друг</span><span class="sxs-lookup"><span data-stu-id="db912-111">currencies</span></span> |<span data-ttu-id="db912-112">Получение валюты.</span><span class="sxs-lookup"><span data-stu-id="db912-112">Get a Currency.</span></span>   |
|[<span data-ttu-id="db912-113">Разноска денежных единиц</span><span class="sxs-lookup"><span data-stu-id="db912-113">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="db912-114">друг</span><span class="sxs-lookup"><span data-stu-id="db912-114">currencies</span></span> |<span data-ttu-id="db912-115">Создание денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="db912-115">Create a Currency.</span></span>|
|[<span data-ttu-id="db912-116">Единицы обновления</span><span class="sxs-lookup"><span data-stu-id="db912-116">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="db912-117">друг</span><span class="sxs-lookup"><span data-stu-id="db912-117">currencies</span></span> |<span data-ttu-id="db912-118">Обновление денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="db912-118">Update a Currency.</span></span>|
|[<span data-ttu-id="db912-119">Удаление валют</span><span class="sxs-lookup"><span data-stu-id="db912-119">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="db912-120">Нет</span><span class="sxs-lookup"><span data-stu-id="db912-120">none</span></span>       |<span data-ttu-id="db912-121">Удаление денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="db912-121">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="db912-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="db912-122">Properties</span></span>
| <span data-ttu-id="db912-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="db912-123">Property</span></span>              | <span data-ttu-id="db912-124">Тип</span><span class="sxs-lookup"><span data-stu-id="db912-124">Type</span></span>   |<span data-ttu-id="db912-125">Описание</span><span class="sxs-lookup"><span data-stu-id="db912-125">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="db912-126">id</span><span class="sxs-lookup"><span data-stu-id="db912-126">id</span></span>                     |<span data-ttu-id="db912-127">GUID</span><span class="sxs-lookup"><span data-stu-id="db912-127">GUID</span></span>    |<span data-ttu-id="db912-128">Уникальный идентификатор валюты.</span><span class="sxs-lookup"><span data-stu-id="db912-128">The unique ID of the currency.</span></span> <span data-ttu-id="db912-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="db912-129">Non-editable.</span></span>                  |
|<span data-ttu-id="db912-130">code</span><span class="sxs-lookup"><span data-stu-id="db912-130">code</span></span>                   |<span data-ttu-id="db912-131">string</span><span class="sxs-lookup"><span data-stu-id="db912-131">string</span></span>  |<span data-ttu-id="db912-132">Указывает код валюты.</span><span class="sxs-lookup"><span data-stu-id="db912-132">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="db912-133">displayName</span><span class="sxs-lookup"><span data-stu-id="db912-133">displayName</span></span>            |<span data-ttu-id="db912-134">string</span><span class="sxs-lookup"><span data-stu-id="db912-134">string</span></span>  |<span data-ttu-id="db912-135">Задает отображаемое имя денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="db912-135">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="db912-136">знаки</span><span class="sxs-lookup"><span data-stu-id="db912-136">symbol</span></span>                 |<span data-ttu-id="db912-137">string</span><span class="sxs-lookup"><span data-stu-id="db912-137">string</span></span>  |<span data-ttu-id="db912-138">Указывает символ валюты, который будет отображаться при проверке.</span><span class="sxs-lookup"><span data-stu-id="db912-138">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="db912-139">амаунтдеЦималплацес</span><span class="sxs-lookup"><span data-stu-id="db912-139">amountDecimalPlaces</span></span>    |<span data-ttu-id="db912-140">string</span><span class="sxs-lookup"><span data-stu-id="db912-140">string</span></span>  |<span data-ttu-id="db912-141">Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.</span><span class="sxs-lookup"><span data-stu-id="db912-141">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="db912-142">амаунтраундингпреЦисион</span><span class="sxs-lookup"><span data-stu-id="db912-142">amountRoundingPrecision</span></span>|<span data-ttu-id="db912-143">числе</span><span class="sxs-lookup"><span data-stu-id="db912-143">decimal</span></span> |<span data-ttu-id="db912-144">Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.</span><span class="sxs-lookup"><span data-stu-id="db912-144">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="db912-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db912-145">lastModifiedDateTime</span></span>   |<span data-ttu-id="db912-146">datetime</span><span class="sxs-lookup"><span data-stu-id="db912-146">datetime</span></span>|<span data-ttu-id="db912-147">Дата и время последнего изменения валюты.</span><span class="sxs-lookup"><span data-stu-id="db912-147">The last datetime the currency was modified.</span></span> <span data-ttu-id="db912-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db912-148">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="db912-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="db912-149">Relationships</span></span>
<span data-ttu-id="db912-150">Нет</span><span class="sxs-lookup"><span data-stu-id="db912-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db912-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db912-151">JSON representation</span></span>

<span data-ttu-id="db912-152">Ниже показано представление валют в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db912-152">Here is a JSON representation of the currencies.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```



