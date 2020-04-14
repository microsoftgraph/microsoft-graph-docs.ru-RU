---
title: Тип ресурса Девицеманажементинтентусерстатесуммари
description: Сущность, представляющая сводную информацию о состоянии пользователя для намерения
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77613d72f616fcaa3e179b56fcea1deed1053aef
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389300"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="ac554-103">Тип ресурса Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="ac554-103">deviceManagementIntentUserStateSummary resource type</span></span>

<span data-ttu-id="ac554-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac554-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac554-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac554-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac554-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac554-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac554-107">Сущность, представляющая сводную информацию о состоянии пользователя для намерения</span><span class="sxs-lookup"><span data-stu-id="ac554-107">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="ac554-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ac554-108">Methods</span></span>
|<span data-ttu-id="ac554-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ac554-109">Method</span></span>|<span data-ttu-id="ac554-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac554-110">Return Type</span></span>|<span data-ttu-id="ac554-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ac554-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac554-112">Получение Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="ac554-112">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="ac554-113">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="ac554-113">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="ac554-114">Чтение свойств и связей объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ac554-114">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="ac554-115">Обновление Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="ac554-115">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="ac554-116">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="ac554-116">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="ac554-117">Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ac554-117">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac554-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac554-118">Properties</span></span>
|<span data-ttu-id="ac554-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac554-119">Property</span></span>|<span data-ttu-id="ac554-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ac554-120">Type</span></span>|<span data-ttu-id="ac554-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ac554-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac554-122">id</span><span class="sxs-lookup"><span data-stu-id="ac554-122">id</span></span>|<span data-ttu-id="ac554-123">String</span><span class="sxs-lookup"><span data-stu-id="ac554-123">String</span></span>|<span data-ttu-id="ac554-124">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ac554-124">The ID</span></span>|
|<span data-ttu-id="ac554-125">conflictCount</span><span class="sxs-lookup"><span data-stu-id="ac554-125">conflictCount</span></span>|<span data-ttu-id="ac554-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ac554-126">Int32</span></span>|<span data-ttu-id="ac554-127">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="ac554-127">Number of users in conflict</span></span>|
|<span data-ttu-id="ac554-128">errorCount</span><span class="sxs-lookup"><span data-stu-id="ac554-128">errorCount</span></span>|<span data-ttu-id="ac554-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ac554-129">Int32</span></span>|<span data-ttu-id="ac554-130">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="ac554-130">Number of error users</span></span>|
|<span data-ttu-id="ac554-131">failedCount</span><span class="sxs-lookup"><span data-stu-id="ac554-131">failedCount</span></span>|<span data-ttu-id="ac554-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ac554-132">Int32</span></span>|<span data-ttu-id="ac554-133">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="ac554-133">Number of failed users</span></span>|
|<span data-ttu-id="ac554-134">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="ac554-134">notApplicableCount</span></span>|<span data-ttu-id="ac554-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ac554-135">Int32</span></span>|<span data-ttu-id="ac554-136">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="ac554-136">Number of not applicable users</span></span>|
|<span data-ttu-id="ac554-137">successCount</span><span class="sxs-lookup"><span data-stu-id="ac554-137">successCount</span></span>|<span data-ttu-id="ac554-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ac554-138">Int32</span></span>|<span data-ttu-id="ac554-139">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="ac554-139">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac554-140">Связи</span><span class="sxs-lookup"><span data-stu-id="ac554-140">Relationships</span></span>
<span data-ttu-id="ac554-141">Нет</span><span class="sxs-lookup"><span data-stu-id="ac554-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac554-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac554-142">JSON Representation</span></span>
<span data-ttu-id="ac554-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac554-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```



