---
title: Тип ресурса deviceComplianceUserOverview
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 01596e7b4e5c4d5a661befadbffa00529d3314d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973197"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="59523-103">Тип ресурса deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="59523-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="59523-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59523-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59523-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="59523-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="59523-106">Методы</span><span class="sxs-lookup"><span data-stu-id="59523-106">Methods</span></span>
|<span data-ttu-id="59523-107">Метод</span><span class="sxs-lookup"><span data-stu-id="59523-107">Method</span></span>|<span data-ttu-id="59523-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="59523-108">Return Type</span></span>|<span data-ttu-id="59523-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59523-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59523-110">Получение объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="59523-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="59523-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="59523-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="59523-112">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="59523-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="59523-113">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="59523-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="59523-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="59523-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="59523-115">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="59523-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59523-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="59523-116">Properties</span></span>
|<span data-ttu-id="59523-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="59523-117">Property</span></span>|<span data-ttu-id="59523-118">Тип</span><span class="sxs-lookup"><span data-stu-id="59523-118">Type</span></span>|<span data-ttu-id="59523-119">Описание</span><span class="sxs-lookup"><span data-stu-id="59523-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59523-120">id</span><span class="sxs-lookup"><span data-stu-id="59523-120">id</span></span>|<span data-ttu-id="59523-121">Строка</span><span class="sxs-lookup"><span data-stu-id="59523-121">String</span></span>|<span data-ttu-id="59523-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59523-122">Key of the entity.</span></span>|
|<span data-ttu-id="59523-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="59523-123">pendingCount</span></span>|<span data-ttu-id="59523-124">Int32</span><span class="sxs-lookup"><span data-stu-id="59523-124">Int32</span></span>|<span data-ttu-id="59523-125">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="59523-125">Number of pending Users</span></span>|
|<span data-ttu-id="59523-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="59523-126">notApplicableCount</span></span>|<span data-ttu-id="59523-127">Int32</span><span class="sxs-lookup"><span data-stu-id="59523-127">Int32</span></span>|<span data-ttu-id="59523-128">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="59523-128">Number of not applicable users</span></span>|
|<span data-ttu-id="59523-129">successCount</span><span class="sxs-lookup"><span data-stu-id="59523-129">successCount</span></span>|<span data-ttu-id="59523-130">Int32</span><span class="sxs-lookup"><span data-stu-id="59523-130">Int32</span></span>|<span data-ttu-id="59523-131">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="59523-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="59523-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="59523-132">errorCount</span></span>|<span data-ttu-id="59523-133">Int32</span><span class="sxs-lookup"><span data-stu-id="59523-133">Int32</span></span>|<span data-ttu-id="59523-134">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="59523-134">Number of error Users</span></span>|
|<span data-ttu-id="59523-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="59523-135">failedCount</span></span>|<span data-ttu-id="59523-136">Int32</span><span class="sxs-lookup"><span data-stu-id="59523-136">Int32</span></span>|<span data-ttu-id="59523-137">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="59523-137">Number of failed Users</span></span>|
|<span data-ttu-id="59523-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="59523-138">lastUpdateDateTime</span></span>|<span data-ttu-id="59523-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59523-139">DateTimeOffset</span></span>|<span data-ttu-id="59523-140">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="59523-140">Last update time</span></span>|
|<span data-ttu-id="59523-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="59523-141">configurationVersion</span></span>|<span data-ttu-id="59523-142">Int32</span><span class="sxs-lookup"><span data-stu-id="59523-142">Int32</span></span>|<span data-ttu-id="59523-143">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="59523-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="59523-144">Связи</span><span class="sxs-lookup"><span data-stu-id="59523-144">Relationships</span></span>
<span data-ttu-id="59523-145">Нет</span><span class="sxs-lookup"><span data-stu-id="59523-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59523-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59523-146">JSON Representation</span></span>
<span data-ttu-id="59523-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59523-147">Here is a JSON representation of the resource.</span></span>
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



