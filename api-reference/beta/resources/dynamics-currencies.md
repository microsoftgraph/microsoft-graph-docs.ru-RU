---
title: Тип ресурса "валюты"
description: Объект Currency в Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543072"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="7eec7-103">Тип ресурса "валюты"</span><span class="sxs-lookup"><span data-stu-id="7eec7-103">currencies resource type</span></span>
<span data-ttu-id="7eec7-104">Представляет валюту, используемую в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="7eec7-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7eec7-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7eec7-105">Methods</span></span>
| <span data-ttu-id="7eec7-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7eec7-106">Method</span></span>                                                  |<span data-ttu-id="7eec7-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7eec7-107">Return Type</span></span>|<span data-ttu-id="7eec7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7eec7-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="7eec7-109">Получение валют</span><span class="sxs-lookup"><span data-stu-id="7eec7-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="7eec7-110">друг</span><span class="sxs-lookup"><span data-stu-id="7eec7-110">currencies</span></span> |<span data-ttu-id="7eec7-111">Получение валюты.</span><span class="sxs-lookup"><span data-stu-id="7eec7-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="7eec7-112">Разноска денежных единиц</span><span class="sxs-lookup"><span data-stu-id="7eec7-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="7eec7-113">друг</span><span class="sxs-lookup"><span data-stu-id="7eec7-113">currencies</span></span> |<span data-ttu-id="7eec7-114">Создание денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="7eec7-114">Create a Currency.</span></span>|
|[<span data-ttu-id="7eec7-115">Единицы обновления</span><span class="sxs-lookup"><span data-stu-id="7eec7-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="7eec7-116">друг</span><span class="sxs-lookup"><span data-stu-id="7eec7-116">currencies</span></span> |<span data-ttu-id="7eec7-117">Обновление денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="7eec7-117">Update a Currency.</span></span>|
|[<span data-ttu-id="7eec7-118">Удаление валют</span><span class="sxs-lookup"><span data-stu-id="7eec7-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="7eec7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7eec7-119">none</span></span>       |<span data-ttu-id="7eec7-120">Удаление денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="7eec7-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="7eec7-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="7eec7-121">Properties</span></span>
| <span data-ttu-id="7eec7-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="7eec7-122">Property</span></span>              | <span data-ttu-id="7eec7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7eec7-123">Type</span></span>   |<span data-ttu-id="7eec7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7eec7-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="7eec7-125">id</span><span class="sxs-lookup"><span data-stu-id="7eec7-125">id</span></span>                     |<span data-ttu-id="7eec7-126">Глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="7eec7-126">GUID</span></span>    |<span data-ttu-id="7eec7-127">Уникальный идентификатор валюты.</span><span class="sxs-lookup"><span data-stu-id="7eec7-127">The unique ID of the currency.</span></span> <span data-ttu-id="7eec7-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="7eec7-128">Non-editable.</span></span>                  |
|<span data-ttu-id="7eec7-129">code</span><span class="sxs-lookup"><span data-stu-id="7eec7-129">code</span></span>                   |<span data-ttu-id="7eec7-130">string</span><span class="sxs-lookup"><span data-stu-id="7eec7-130">string</span></span>  |<span data-ttu-id="7eec7-131">Указывает код валюты.</span><span class="sxs-lookup"><span data-stu-id="7eec7-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="7eec7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7eec7-132">displayName</span></span>            |<span data-ttu-id="7eec7-133">string</span><span class="sxs-lookup"><span data-stu-id="7eec7-133">string</span></span>  |<span data-ttu-id="7eec7-134">Задает отображаемое имя денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="7eec7-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="7eec7-135">знаки</span><span class="sxs-lookup"><span data-stu-id="7eec7-135">symbol</span></span>                 |<span data-ttu-id="7eec7-136">string</span><span class="sxs-lookup"><span data-stu-id="7eec7-136">string</span></span>  |<span data-ttu-id="7eec7-137">Указывает символ валюты, который будет отображаться при проверке.</span><span class="sxs-lookup"><span data-stu-id="7eec7-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="7eec7-138">АмаунтдеЦималплацес</span><span class="sxs-lookup"><span data-stu-id="7eec7-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="7eec7-139">string</span><span class="sxs-lookup"><span data-stu-id="7eec7-139">string</span></span>  |<span data-ttu-id="7eec7-140">Указывает количество десятичных разрядов, отображаемых системой на суммах для этой валюты.</span><span class="sxs-lookup"><span data-stu-id="7eec7-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="7eec7-141">АмаунтраундингпреЦисион</span><span class="sxs-lookup"><span data-stu-id="7eec7-141">amountRoundingPrecision</span></span>|<span data-ttu-id="7eec7-142">числе</span><span class="sxs-lookup"><span data-stu-id="7eec7-142">decimal</span></span> |<span data-ttu-id="7eec7-143">Указывает размер интервала, который будет использоваться при округлении сумм для данной валюты.</span><span class="sxs-lookup"><span data-stu-id="7eec7-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="7eec7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7eec7-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="7eec7-145">отличным</span><span class="sxs-lookup"><span data-stu-id="7eec7-145">datetime</span></span>|<span data-ttu-id="7eec7-146">Дата и время последнего изменения валюты.</span><span class="sxs-lookup"><span data-stu-id="7eec7-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="7eec7-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7eec7-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="7eec7-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="7eec7-148">Relationships</span></span>
<span data-ttu-id="7eec7-149">Нет</span><span class="sxs-lookup"><span data-stu-id="7eec7-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7eec7-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7eec7-150">JSON representation</span></span>

<span data-ttu-id="7eec7-151">Ниже показано представление валют в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7eec7-151">Here is a JSON representation of the currencies.</span></span>


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

