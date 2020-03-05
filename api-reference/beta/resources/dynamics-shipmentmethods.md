---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 94ebd10ef87946b5333ec5a06d5edccadc298158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503574"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="cab90-103">Тип ресурса Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-103">shipmentMethods resource type</span></span>

<span data-ttu-id="cab90-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cab90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cab90-105">Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.</span><span class="sxs-lookup"><span data-stu-id="cab90-105">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="cab90-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cab90-106">Methods</span></span>

| <span data-ttu-id="cab90-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cab90-107">Method</span></span>       | <span data-ttu-id="cab90-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cab90-108">Return Type</span></span>  |<span data-ttu-id="cab90-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cab90-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cab90-110">Получение Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-110">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="cab90-111">шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-111">shipmentMethods</span></span>|<span data-ttu-id="cab90-112">Получает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-112">Gets a shipment method.</span></span>|
|[<span data-ttu-id="cab90-113">POST Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-113">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="cab90-114">шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-114">shipmentMethods</span></span>|<span data-ttu-id="cab90-115">Создает метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-115">Creates a shipment method.</span></span>|
|[<span data-ttu-id="cab90-116">Исправление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-116">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="cab90-117">шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-117">shipmentMethods</span></span>|<span data-ttu-id="cab90-118">Обновляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-118">Updates a shipment method.</span></span>|
|[<span data-ttu-id="cab90-119">Удаление Шипментмесодс</span><span class="sxs-lookup"><span data-stu-id="cab90-119">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="cab90-120">нет</span><span class="sxs-lookup"><span data-stu-id="cab90-120">none</span></span>|<span data-ttu-id="cab90-121">Удаляет метод отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-121">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="cab90-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="cab90-122">Properties</span></span>
| <span data-ttu-id="cab90-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="cab90-123">Property</span></span>     | <span data-ttu-id="cab90-124">Тип</span><span class="sxs-lookup"><span data-stu-id="cab90-124">Type</span></span>   |<span data-ttu-id="cab90-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cab90-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cab90-126">id</span><span class="sxs-lookup"><span data-stu-id="cab90-126">id</span></span>|<span data-ttu-id="cab90-127">GUID</span><span class="sxs-lookup"><span data-stu-id="cab90-127">GUID</span></span>|<span data-ttu-id="cab90-128">Уникальный идентификатор Шипментмесод.</span><span class="sxs-lookup"><span data-stu-id="cab90-128">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="cab90-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="cab90-129">Non-editable.</span></span>|
|<span data-ttu-id="cab90-130">code</span><span class="sxs-lookup"><span data-stu-id="cab90-130">code</span></span>|<span data-ttu-id="cab90-131">string</span><span class="sxs-lookup"><span data-stu-id="cab90-131">string</span></span>|<span data-ttu-id="cab90-132">Указывает код метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-132">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="cab90-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cab90-133">displayName</span></span>|<span data-ttu-id="cab90-134">string</span><span class="sxs-lookup"><span data-stu-id="cab90-134">string</span></span>|<span data-ttu-id="cab90-135">Задает отображаемое имя метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-135">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="cab90-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cab90-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cab90-137">datetime</span><span class="sxs-lookup"><span data-stu-id="cab90-137">datetime</span></span>|<span data-ttu-id="cab90-138">Дата и время последнего изменения метода отгрузки.</span><span class="sxs-lookup"><span data-stu-id="cab90-138">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="cab90-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cab90-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="cab90-140">Связи</span><span class="sxs-lookup"><span data-stu-id="cab90-140">Relationships</span></span>
<span data-ttu-id="cab90-141">Нет</span><span class="sxs-lookup"><span data-stu-id="cab90-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cab90-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cab90-142">JSON representation</span></span>

<span data-ttu-id="cab90-143">Ниже показано представление объекта Шипментмесод в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cab90-143">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


