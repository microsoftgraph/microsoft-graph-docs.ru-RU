---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ba8ad750831394e2a84fab7ca87d76754838db60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012620"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="80b2e-103">Тип ресурса "валюты"</span><span class="sxs-lookup"><span data-stu-id="80b2e-103">currencies resource type</span></span>
<span data-ttu-id="80b2e-104">Представляет валюту, используемую в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="80b2e-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="80b2e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="80b2e-105">Methods</span></span>
| <span data-ttu-id="80b2e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="80b2e-106">Method</span></span>                                                  |<span data-ttu-id="80b2e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="80b2e-107">Return Type</span></span>|<span data-ttu-id="80b2e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="80b2e-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="80b2e-109">Получение валют</span><span class="sxs-lookup"><span data-stu-id="80b2e-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="80b2e-110">друг</span><span class="sxs-lookup"><span data-stu-id="80b2e-110">currencies</span></span> |<span data-ttu-id="80b2e-111">Получение валюты.</span><span class="sxs-lookup"><span data-stu-id="80b2e-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="80b2e-112">Разноска денежных единиц</span><span class="sxs-lookup"><span data-stu-id="80b2e-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="80b2e-113">друг</span><span class="sxs-lookup"><span data-stu-id="80b2e-113">currencies</span></span> |<span data-ttu-id="80b2e-114">Создание денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="80b2e-114">Create a Currency.</span></span>|
|[<span data-ttu-id="80b2e-115">Единицы обновления</span><span class="sxs-lookup"><span data-stu-id="80b2e-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="80b2e-116">друг</span><span class="sxs-lookup"><span data-stu-id="80b2e-116">currencies</span></span> |<span data-ttu-id="80b2e-117">Обновление денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="80b2e-117">Update a Currency.</span></span>|
|[<span data-ttu-id="80b2e-118">Удаление валют</span><span class="sxs-lookup"><span data-stu-id="80b2e-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="80b2e-119">none</span><span class="sxs-lookup"><span data-stu-id="80b2e-119">none</span></span>       |<span data-ttu-id="80b2e-120">Удаление денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="80b2e-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="80b2e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="80b2e-121">Properties</span></span>
| <span data-ttu-id="80b2e-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="80b2e-122">Property</span></span>              | <span data-ttu-id="80b2e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="80b2e-123">Type</span></span>   |<span data-ttu-id="80b2e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="80b2e-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="80b2e-125">id</span><span class="sxs-lookup"><span data-stu-id="80b2e-125">id</span></span>                     |<span data-ttu-id="80b2e-126">GUID</span><span class="sxs-lookup"><span data-stu-id="80b2e-126">GUID</span></span>    |<span data-ttu-id="80b2e-127">Уникальный идентификатор валюты.</span><span class="sxs-lookup"><span data-stu-id="80b2e-127">The unique ID of the currency.</span></span> <span data-ttu-id="80b2e-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="80b2e-128">Non-editable.</span></span>                  |
|<span data-ttu-id="80b2e-129">code</span><span class="sxs-lookup"><span data-stu-id="80b2e-129">code</span></span>                   |<span data-ttu-id="80b2e-130">string</span><span class="sxs-lookup"><span data-stu-id="80b2e-130">string</span></span>  |<span data-ttu-id="80b2e-131">Указывает код валюты.</span><span class="sxs-lookup"><span data-stu-id="80b2e-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="80b2e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="80b2e-132">displayName</span></span>            |<span data-ttu-id="80b2e-133">string</span><span class="sxs-lookup"><span data-stu-id="80b2e-133">string</span></span>  |<span data-ttu-id="80b2e-134">Задает отображаемое имя денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="80b2e-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="80b2e-135">знаки</span><span class="sxs-lookup"><span data-stu-id="80b2e-135">symbol</span></span>                 |<span data-ttu-id="80b2e-136">string</span><span class="sxs-lookup"><span data-stu-id="80b2e-136">string</span></span>  |<span data-ttu-id="80b2e-137">Указывает символ валюты, который будет отображаться при проверке.</span><span class="sxs-lookup"><span data-stu-id="80b2e-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="80b2e-138">АмаунтдеЦималплацес</span><span class="sxs-lookup"><span data-stu-id="80b2e-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="80b2e-139">string</span><span class="sxs-lookup"><span data-stu-id="80b2e-139">string</span></span>  |<span data-ttu-id="80b2e-140">Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.</span><span class="sxs-lookup"><span data-stu-id="80b2e-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="80b2e-141">АмаунтраундингпреЦисион</span><span class="sxs-lookup"><span data-stu-id="80b2e-141">amountRoundingPrecision</span></span>|<span data-ttu-id="80b2e-142">числе</span><span class="sxs-lookup"><span data-stu-id="80b2e-142">decimal</span></span> |<span data-ttu-id="80b2e-143">Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.</span><span class="sxs-lookup"><span data-stu-id="80b2e-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="80b2e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80b2e-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="80b2e-145">отличным</span><span class="sxs-lookup"><span data-stu-id="80b2e-145">datetime</span></span>|<span data-ttu-id="80b2e-146">Дата и время последнего изменения валюты.</span><span class="sxs-lookup"><span data-stu-id="80b2e-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="80b2e-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80b2e-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="80b2e-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="80b2e-148">Relationships</span></span>
<span data-ttu-id="80b2e-149">Нет</span><span class="sxs-lookup"><span data-stu-id="80b2e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80b2e-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80b2e-150">JSON representation</span></span>

<span data-ttu-id="80b2e-151">Ниже показано представление валют в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80b2e-151">Here is a JSON representation of the currencies.</span></span>


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

