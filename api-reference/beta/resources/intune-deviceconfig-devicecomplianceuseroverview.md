---
title: Тип ресурса deviceComplianceUserOverview
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 6505cf0d563f129d4a683026f5dc828310c32792
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359390"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="51350-103">Тип ресурса deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="51350-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="51350-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51350-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51350-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51350-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51350-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51350-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51350-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="51350-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="51350-108">Методы</span><span class="sxs-lookup"><span data-stu-id="51350-108">Methods</span></span>
|<span data-ttu-id="51350-109">Метод</span><span class="sxs-lookup"><span data-stu-id="51350-109">Method</span></span>|<span data-ttu-id="51350-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51350-110">Return Type</span></span>|<span data-ttu-id="51350-111">Описание</span><span class="sxs-lookup"><span data-stu-id="51350-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51350-112">Получение объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="51350-112">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="51350-113">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="51350-113">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="51350-114">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="51350-114">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="51350-115">Обновление объекта deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="51350-115">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="51350-116">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="51350-116">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="51350-117">Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="51350-117">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51350-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="51350-118">Properties</span></span>
|<span data-ttu-id="51350-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="51350-119">Property</span></span>|<span data-ttu-id="51350-120">Тип</span><span class="sxs-lookup"><span data-stu-id="51350-120">Type</span></span>|<span data-ttu-id="51350-121">Описание</span><span class="sxs-lookup"><span data-stu-id="51350-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51350-122">id</span><span class="sxs-lookup"><span data-stu-id="51350-122">id</span></span>|<span data-ttu-id="51350-123">Строка</span><span class="sxs-lookup"><span data-stu-id="51350-123">String</span></span>|<span data-ttu-id="51350-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51350-124">Key of the entity.</span></span>|
|<span data-ttu-id="51350-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="51350-125">pendingCount</span></span>|<span data-ttu-id="51350-126">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-126">Int32</span></span>|<span data-ttu-id="51350-127">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="51350-127">Number of pending Users</span></span>|
|<span data-ttu-id="51350-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="51350-128">notApplicableCount</span></span>|<span data-ttu-id="51350-129">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-129">Int32</span></span>|<span data-ttu-id="51350-130">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="51350-130">Number of not applicable users</span></span>|
|<span data-ttu-id="51350-131">successCount</span><span class="sxs-lookup"><span data-stu-id="51350-131">successCount</span></span>|<span data-ttu-id="51350-132">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-132">Int32</span></span>|<span data-ttu-id="51350-133">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="51350-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="51350-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="51350-134">errorCount</span></span>|<span data-ttu-id="51350-135">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-135">Int32</span></span>|<span data-ttu-id="51350-136">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="51350-136">Number of error Users</span></span>|
|<span data-ttu-id="51350-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="51350-137">failedCount</span></span>|<span data-ttu-id="51350-138">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-138">Int32</span></span>|<span data-ttu-id="51350-139">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="51350-139">Number of failed Users</span></span>|
|<span data-ttu-id="51350-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="51350-140">conflictCount</span></span>|<span data-ttu-id="51350-141">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-141">Int32</span></span>|<span data-ttu-id="51350-142">Количество пользователей в конфликта</span><span class="sxs-lookup"><span data-stu-id="51350-142">Number of users in conflict</span></span>|
|<span data-ttu-id="51350-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="51350-143">lastUpdateDateTime</span></span>|<span data-ttu-id="51350-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51350-144">DateTimeOffset</span></span>|<span data-ttu-id="51350-145">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="51350-145">Last update time</span></span>|
|<span data-ttu-id="51350-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="51350-146">configurationVersion</span></span>|<span data-ttu-id="51350-147">Int32</span><span class="sxs-lookup"><span data-stu-id="51350-147">Int32</span></span>|<span data-ttu-id="51350-148">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="51350-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="51350-149">Связи</span><span class="sxs-lookup"><span data-stu-id="51350-149">Relationships</span></span>
<span data-ttu-id="51350-150">Нет</span><span class="sxs-lookup"><span data-stu-id="51350-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51350-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51350-151">JSON Representation</span></span>
<span data-ttu-id="51350-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51350-152">Here is a JSON representation of the resource.</span></span>
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
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





