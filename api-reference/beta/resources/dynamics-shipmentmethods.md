---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e8d25294b219815c8aa569c7a8c7fab7ec68830c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006614"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="907f3-103">Тип ресурса Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-103">shipmentMethods resource type</span></span>
<span data-ttu-id="907f3-104">Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.</span><span class="sxs-lookup"><span data-stu-id="907f3-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="907f3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="907f3-105">Methods</span></span>

| <span data-ttu-id="907f3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="907f3-106">Method</span></span>       | <span data-ttu-id="907f3-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="907f3-107">Return Type</span></span>  |<span data-ttu-id="907f3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="907f3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="907f3-109">Получение Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="907f3-110">Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-110">shipmentMethods</span></span>|<span data-ttu-id="907f3-111">Получает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="907f3-112">POST Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="907f3-113">Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-113">shipmentMethods</span></span>|<span data-ttu-id="907f3-114">Создает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="907f3-115">Исправление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="907f3-116">Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-116">shipmentMethods</span></span>|<span data-ttu-id="907f3-117">Обновляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="907f3-118">Удаление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="907f3-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="907f3-119">none</span><span class="sxs-lookup"><span data-stu-id="907f3-119">none</span></span>|<span data-ttu-id="907f3-120">Удаляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="907f3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="907f3-121">Properties</span></span>
| <span data-ttu-id="907f3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="907f3-122">Property</span></span>     | <span data-ttu-id="907f3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="907f3-123">Type</span></span>   |<span data-ttu-id="907f3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="907f3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="907f3-125">id</span><span class="sxs-lookup"><span data-stu-id="907f3-125">id</span></span>|<span data-ttu-id="907f3-126">GUID</span><span class="sxs-lookup"><span data-stu-id="907f3-126">GUID</span></span>|<span data-ttu-id="907f3-127">Уникальный идентификатор Шипментмесод.</span><span class="sxs-lookup"><span data-stu-id="907f3-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="907f3-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="907f3-128">Non-editable.</span></span>|
|<span data-ttu-id="907f3-129">code</span><span class="sxs-lookup"><span data-stu-id="907f3-129">code</span></span>|<span data-ttu-id="907f3-130">string</span><span class="sxs-lookup"><span data-stu-id="907f3-130">string</span></span>|<span data-ttu-id="907f3-131">Указывает код метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="907f3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="907f3-132">displayName</span></span>|<span data-ttu-id="907f3-133">string</span><span class="sxs-lookup"><span data-stu-id="907f3-133">string</span></span>|<span data-ttu-id="907f3-134">Задает отображаемое имя метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="907f3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="907f3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="907f3-136">отличным</span><span class="sxs-lookup"><span data-stu-id="907f3-136">datetime</span></span>|<span data-ttu-id="907f3-137">Дата и время последнего изменения метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="907f3-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="907f3-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="907f3-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="907f3-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="907f3-139">Relationships</span></span>
<span data-ttu-id="907f3-140">Нет</span><span class="sxs-lookup"><span data-stu-id="907f3-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="907f3-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="907f3-141">JSON representation</span></span>

<span data-ttu-id="907f3-142">Ниже показано представление объекта Шипментмесод в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="907f3-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


