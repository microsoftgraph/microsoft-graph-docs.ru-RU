---
title: Тип ресурса deviceConfigurationUserOverview
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c20471630b2ab888af96a33b1e24eced26d3015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926304"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="059b5-103">Тип ресурса deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="059b5-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="059b5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="059b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="059b5-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="059b5-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="059b5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="059b5-106">Methods</span></span>
|<span data-ttu-id="059b5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="059b5-107">Method</span></span>|<span data-ttu-id="059b5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="059b5-108">Return Type</span></span>|<span data-ttu-id="059b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="059b5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="059b5-110">Получение объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="059b5-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="059b5-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="059b5-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="059b5-112">Чтение свойств и связей объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="059b5-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="059b5-113">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="059b5-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="059b5-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="059b5-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="059b5-115">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="059b5-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="059b5-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="059b5-116">Properties</span></span>
|<span data-ttu-id="059b5-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="059b5-117">Property</span></span>|<span data-ttu-id="059b5-118">Тип</span><span class="sxs-lookup"><span data-stu-id="059b5-118">Type</span></span>|<span data-ttu-id="059b5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="059b5-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="059b5-120">id</span><span class="sxs-lookup"><span data-stu-id="059b5-120">id</span></span>|<span data-ttu-id="059b5-121">Строка</span><span class="sxs-lookup"><span data-stu-id="059b5-121">String</span></span>|<span data-ttu-id="059b5-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="059b5-122">Key of the entity.</span></span>|
|<span data-ttu-id="059b5-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="059b5-123">pendingCount</span></span>|<span data-ttu-id="059b5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="059b5-124">Int32</span></span>|<span data-ttu-id="059b5-125">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="059b5-125">Number of pending Users</span></span>|
|<span data-ttu-id="059b5-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="059b5-126">notApplicableCount</span></span>|<span data-ttu-id="059b5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="059b5-127">Int32</span></span>|<span data-ttu-id="059b5-128">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="059b5-128">Number of not applicable users</span></span>|
|<span data-ttu-id="059b5-129">successCount</span><span class="sxs-lookup"><span data-stu-id="059b5-129">successCount</span></span>|<span data-ttu-id="059b5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="059b5-130">Int32</span></span>|<span data-ttu-id="059b5-131">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="059b5-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="059b5-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="059b5-132">errorCount</span></span>|<span data-ttu-id="059b5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="059b5-133">Int32</span></span>|<span data-ttu-id="059b5-134">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="059b5-134">Number of error Users</span></span>|
|<span data-ttu-id="059b5-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="059b5-135">failedCount</span></span>|<span data-ttu-id="059b5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="059b5-136">Int32</span></span>|<span data-ttu-id="059b5-137">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="059b5-137">Number of failed Users</span></span>|
|<span data-ttu-id="059b5-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="059b5-138">lastUpdateDateTime</span></span>|<span data-ttu-id="059b5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="059b5-139">DateTimeOffset</span></span>|<span data-ttu-id="059b5-140">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="059b5-140">Last update time</span></span>|
|<span data-ttu-id="059b5-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="059b5-141">configurationVersion</span></span>|<span data-ttu-id="059b5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="059b5-142">Int32</span></span>|<span data-ttu-id="059b5-143">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="059b5-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="059b5-144">Связи</span><span class="sxs-lookup"><span data-stu-id="059b5-144">Relationships</span></span>
<span data-ttu-id="059b5-145">Нет</span><span class="sxs-lookup"><span data-stu-id="059b5-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="059b5-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="059b5-146">JSON Representation</span></span>
<span data-ttu-id="059b5-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="059b5-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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



