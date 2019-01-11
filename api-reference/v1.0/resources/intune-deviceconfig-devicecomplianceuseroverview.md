---
title: Тип ресурса deviceComplianceUserOverview
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31b5666fd7d99c3ff71819ef06c144dd14550167
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817565"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="1e080-103">Тип ресурса deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="1e080-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="1e080-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e080-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e080-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1e080-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1e080-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1e080-106">Methods</span></span>
|<span data-ttu-id="1e080-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1e080-107">Method</span></span>|<span data-ttu-id="1e080-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e080-108">Return Type</span></span>|<span data-ttu-id="1e080-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e080-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e080-110">Получение объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="1e080-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="1e080-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="1e080-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="1e080-112">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="1e080-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="1e080-113">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="1e080-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="1e080-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="1e080-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="1e080-115">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="1e080-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e080-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e080-116">Properties</span></span>
|<span data-ttu-id="1e080-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e080-117">Property</span></span>|<span data-ttu-id="1e080-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1e080-118">Type</span></span>|<span data-ttu-id="1e080-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1e080-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e080-120">id</span><span class="sxs-lookup"><span data-stu-id="1e080-120">id</span></span>|<span data-ttu-id="1e080-121">Строка</span><span class="sxs-lookup"><span data-stu-id="1e080-121">String</span></span>|<span data-ttu-id="1e080-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1e080-122">Key of the entity.</span></span>|
|<span data-ttu-id="1e080-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1e080-123">pendingCount</span></span>|<span data-ttu-id="1e080-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1e080-124">Int32</span></span>|<span data-ttu-id="1e080-125">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="1e080-125">Number of pending Users</span></span>|
|<span data-ttu-id="1e080-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1e080-126">notApplicableCount</span></span>|<span data-ttu-id="1e080-127">Int32</span><span class="sxs-lookup"><span data-stu-id="1e080-127">Int32</span></span>|<span data-ttu-id="1e080-128">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="1e080-128">Number of not applicable users</span></span>|
|<span data-ttu-id="1e080-129">successCount</span><span class="sxs-lookup"><span data-stu-id="1e080-129">successCount</span></span>|<span data-ttu-id="1e080-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1e080-130">Int32</span></span>|<span data-ttu-id="1e080-131">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1e080-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="1e080-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="1e080-132">errorCount</span></span>|<span data-ttu-id="1e080-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1e080-133">Int32</span></span>|<span data-ttu-id="1e080-134">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1e080-134">Number of error Users</span></span>|
|<span data-ttu-id="1e080-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="1e080-135">failedCount</span></span>|<span data-ttu-id="1e080-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1e080-136">Int32</span></span>|<span data-ttu-id="1e080-137">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="1e080-137">Number of failed Users</span></span>|
|<span data-ttu-id="1e080-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1e080-138">lastUpdateDateTime</span></span>|<span data-ttu-id="1e080-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e080-139">DateTimeOffset</span></span>|<span data-ttu-id="1e080-140">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="1e080-140">Last update time</span></span>|
|<span data-ttu-id="1e080-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1e080-141">configurationVersion</span></span>|<span data-ttu-id="1e080-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1e080-142">Int32</span></span>|<span data-ttu-id="1e080-143">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="1e080-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e080-144">Связи</span><span class="sxs-lookup"><span data-stu-id="1e080-144">Relationships</span></span>
<span data-ttu-id="1e080-145">Нет</span><span class="sxs-lookup"><span data-stu-id="1e080-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e080-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e080-146">JSON Representation</span></span>
<span data-ttu-id="1e080-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e080-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



