---
title: Тип ресурса deviceConfigurationUserOverview
description: Н/Д
ms.openlocfilehash: ba2ac821aa63d3a008e95a5f36b3c75285c2b6cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025383"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="164de-103">Тип ресурса deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="164de-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="164de-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="164de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="164de-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="164de-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="164de-106">Методы</span><span class="sxs-lookup"><span data-stu-id="164de-106">Methods</span></span>
|<span data-ttu-id="164de-107">Метод</span><span class="sxs-lookup"><span data-stu-id="164de-107">Method</span></span>|<span data-ttu-id="164de-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="164de-108">Return Type</span></span>|<span data-ttu-id="164de-109">Описание</span><span class="sxs-lookup"><span data-stu-id="164de-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="164de-110">Получение объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="164de-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="164de-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="164de-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="164de-112">Чтение свойств и связей объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="164de-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="164de-113">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="164de-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="164de-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="164de-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="164de-115">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="164de-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="164de-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="164de-116">Properties</span></span>
|<span data-ttu-id="164de-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="164de-117">Property</span></span>|<span data-ttu-id="164de-118">Тип</span><span class="sxs-lookup"><span data-stu-id="164de-118">Type</span></span>|<span data-ttu-id="164de-119">Описание</span><span class="sxs-lookup"><span data-stu-id="164de-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="164de-120">id</span><span class="sxs-lookup"><span data-stu-id="164de-120">id</span></span>|<span data-ttu-id="164de-121">String</span><span class="sxs-lookup"><span data-stu-id="164de-121">String</span></span>|<span data-ttu-id="164de-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="164de-122">Key of the entity.</span></span>|
|<span data-ttu-id="164de-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="164de-123">pendingCount</span></span>|<span data-ttu-id="164de-124">Int32</span><span class="sxs-lookup"><span data-stu-id="164de-124">Int32</span></span>|<span data-ttu-id="164de-125">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="164de-125">Number of pending Users</span></span>|
|<span data-ttu-id="164de-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="164de-126">notApplicableCount</span></span>|<span data-ttu-id="164de-127">Int32</span><span class="sxs-lookup"><span data-stu-id="164de-127">Int32</span></span>|<span data-ttu-id="164de-128">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="164de-128">Number of not applicable users</span></span>|
|<span data-ttu-id="164de-129">successCount</span><span class="sxs-lookup"><span data-stu-id="164de-129">successCount</span></span>|<span data-ttu-id="164de-130">Int32</span><span class="sxs-lookup"><span data-stu-id="164de-130">Int32</span></span>|<span data-ttu-id="164de-131">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="164de-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="164de-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="164de-132">errorCount</span></span>|<span data-ttu-id="164de-133">Int32</span><span class="sxs-lookup"><span data-stu-id="164de-133">Int32</span></span>|<span data-ttu-id="164de-134">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="164de-134">Number of error Users</span></span>|
|<span data-ttu-id="164de-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="164de-135">failedCount</span></span>|<span data-ttu-id="164de-136">Int32</span><span class="sxs-lookup"><span data-stu-id="164de-136">Int32</span></span>|<span data-ttu-id="164de-137">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="164de-137">Number of failed Users</span></span>|
|<span data-ttu-id="164de-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="164de-138">lastUpdateDateTime</span></span>|<span data-ttu-id="164de-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164de-139">DateTimeOffset</span></span>|<span data-ttu-id="164de-140">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="164de-140">Last update time</span></span>|
|<span data-ttu-id="164de-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="164de-141">configurationVersion</span></span>|<span data-ttu-id="164de-142">Int32</span><span class="sxs-lookup"><span data-stu-id="164de-142">Int32</span></span>|<span data-ttu-id="164de-143">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="164de-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="164de-144">Связи</span><span class="sxs-lookup"><span data-stu-id="164de-144">Relationships</span></span>
<span data-ttu-id="164de-145">Нет</span><span class="sxs-lookup"><span data-stu-id="164de-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="164de-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="164de-146">JSON Representation</span></span>
<span data-ttu-id="164de-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="164de-147">Here is a JSON representation of the resource.</span></span>
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



