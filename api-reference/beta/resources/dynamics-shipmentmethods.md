---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d45153a08572f32f29128fd4d3f51638d71c951b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027071"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="fb7ea-103">Тип ресурса Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-103">shipmentMethods resource type</span></span>

<span data-ttu-id="fb7ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb7ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb7ea-105">Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-105">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="fb7ea-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fb7ea-106">Methods</span></span>

| <span data-ttu-id="fb7ea-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fb7ea-107">Method</span></span>       | <span data-ttu-id="fb7ea-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb7ea-108">Return Type</span></span>  |<span data-ttu-id="fb7ea-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fb7ea-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb7ea-110">Получение Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-110">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="fb7ea-111">шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-111">shipmentMethods</span></span>|<span data-ttu-id="fb7ea-112">Получает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-112">Gets a shipment method.</span></span>|
|[<span data-ttu-id="fb7ea-113">POST Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-113">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="fb7ea-114">шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-114">shipmentMethods</span></span>|<span data-ttu-id="fb7ea-115">Создает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-115">Creates a shipment method.</span></span>|
|[<span data-ttu-id="fb7ea-116">Исправление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-116">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="fb7ea-117">шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-117">shipmentMethods</span></span>|<span data-ttu-id="fb7ea-118">Обновляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-118">Updates a shipment method.</span></span>|
|[<span data-ttu-id="fb7ea-119">Удаление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="fb7ea-119">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="fb7ea-120">Нет</span><span class="sxs-lookup"><span data-stu-id="fb7ea-120">none</span></span>|<span data-ttu-id="fb7ea-121">Удаляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-121">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb7ea-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb7ea-122">Properties</span></span>
| <span data-ttu-id="fb7ea-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb7ea-123">Property</span></span>     | <span data-ttu-id="fb7ea-124">Тип</span><span class="sxs-lookup"><span data-stu-id="fb7ea-124">Type</span></span>   |<span data-ttu-id="fb7ea-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fb7ea-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb7ea-126">id</span><span class="sxs-lookup"><span data-stu-id="fb7ea-126">id</span></span>|<span data-ttu-id="fb7ea-127">GUID</span><span class="sxs-lookup"><span data-stu-id="fb7ea-127">GUID</span></span>|<span data-ttu-id="fb7ea-128">Уникальный идентификатор Шипментмесод.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-128">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="fb7ea-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-129">Non-editable.</span></span>|
|<span data-ttu-id="fb7ea-130">code</span><span class="sxs-lookup"><span data-stu-id="fb7ea-130">code</span></span>|<span data-ttu-id="fb7ea-131">string</span><span class="sxs-lookup"><span data-stu-id="fb7ea-131">string</span></span>|<span data-ttu-id="fb7ea-132">Указывает код метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-132">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="fb7ea-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fb7ea-133">displayName</span></span>|<span data-ttu-id="fb7ea-134">string</span><span class="sxs-lookup"><span data-stu-id="fb7ea-134">string</span></span>|<span data-ttu-id="fb7ea-135">Задает отображаемое имя метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-135">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="fb7ea-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb7ea-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fb7ea-137">datetime</span><span class="sxs-lookup"><span data-stu-id="fb7ea-137">datetime</span></span>|<span data-ttu-id="fb7ea-138">Дата и время последнего изменения метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-138">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="fb7ea-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="fb7ea-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="fb7ea-140">Relationships</span></span>
<span data-ttu-id="fb7ea-141">Нет</span><span class="sxs-lookup"><span data-stu-id="fb7ea-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb7ea-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb7ea-142">JSON representation</span></span>

<span data-ttu-id="fb7ea-143">Ниже показано представление объекта Шипментмесод в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb7ea-143">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```




