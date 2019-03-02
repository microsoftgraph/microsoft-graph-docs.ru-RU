---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365502"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="92541-103">Тип ресурса Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-103">shipmentMethods resource type</span></span>
<span data-ttu-id="92541-104">Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.</span><span class="sxs-lookup"><span data-stu-id="92541-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="92541-105">Методы</span><span class="sxs-lookup"><span data-stu-id="92541-105">Methods</span></span>

| <span data-ttu-id="92541-106">Метод</span><span class="sxs-lookup"><span data-stu-id="92541-106">Method</span></span>       | <span data-ttu-id="92541-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92541-107">Return Type</span></span>  |<span data-ttu-id="92541-108">Описание</span><span class="sxs-lookup"><span data-stu-id="92541-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92541-109">Получение Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="92541-110">Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-110">shipmentMethods</span></span>|<span data-ttu-id="92541-111">Получает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="92541-112">POST Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="92541-113">Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-113">shipmentMethods</span></span>|<span data-ttu-id="92541-114">Создает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="92541-115">Исправление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="92541-116">Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-116">shipmentMethods</span></span>|<span data-ttu-id="92541-117">Обновляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="92541-118">Удаление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="92541-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="92541-119">Нет</span><span class="sxs-lookup"><span data-stu-id="92541-119">none</span></span>|<span data-ttu-id="92541-120">Удаляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="92541-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="92541-121">Properties</span></span>
| <span data-ttu-id="92541-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="92541-122">Property</span></span>     | <span data-ttu-id="92541-123">Тип</span><span class="sxs-lookup"><span data-stu-id="92541-123">Type</span></span>   |<span data-ttu-id="92541-124">Описание</span><span class="sxs-lookup"><span data-stu-id="92541-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92541-125">id</span><span class="sxs-lookup"><span data-stu-id="92541-125">id</span></span>|<span data-ttu-id="92541-126">GUID</span><span class="sxs-lookup"><span data-stu-id="92541-126">GUID</span></span>|<span data-ttu-id="92541-127">Уникальный идентификатор Шипментмесод.</span><span class="sxs-lookup"><span data-stu-id="92541-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="92541-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="92541-128">Non-editable.</span></span>|
|<span data-ttu-id="92541-129">code</span><span class="sxs-lookup"><span data-stu-id="92541-129">code</span></span>|<span data-ttu-id="92541-130">строка</span><span class="sxs-lookup"><span data-stu-id="92541-130">string</span></span>|<span data-ttu-id="92541-131">Указывает код метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="92541-132">displayName</span><span class="sxs-lookup"><span data-stu-id="92541-132">displayName</span></span>|<span data-ttu-id="92541-133">строка</span><span class="sxs-lookup"><span data-stu-id="92541-133">string</span></span>|<span data-ttu-id="92541-134">Задает отображаемое имя метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="92541-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92541-135">lastModifiedDateTime</span></span>|<span data-ttu-id="92541-136">отличным</span><span class="sxs-lookup"><span data-stu-id="92541-136">datetime</span></span>|<span data-ttu-id="92541-137">Дата и время последнего изменения метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="92541-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="92541-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92541-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="92541-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="92541-139">Relationships</span></span>
<span data-ttu-id="92541-140">Нет</span><span class="sxs-lookup"><span data-stu-id="92541-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92541-141">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="92541-141">JSON representation</span></span>

<span data-ttu-id="92541-142">Ниже показано представление объекта Шипментмесод в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92541-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


