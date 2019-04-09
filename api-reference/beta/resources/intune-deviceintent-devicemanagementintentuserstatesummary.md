---
title: Тип ресурса Девицеманажементинтентусерстатесуммари
description: Сущность, представляющая сводную информацию о состоянии пользователя для намерения
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c930b19e604aaf3867260e359a2b7fcb12153762
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523996"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="55403-103">Тип ресурса Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="55403-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="55403-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55403-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55403-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55403-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55403-106">Сущность, представляющая сводную информацию о состоянии пользователя для намерения</span><span class="sxs-lookup"><span data-stu-id="55403-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="55403-107">Методы</span><span class="sxs-lookup"><span data-stu-id="55403-107">Methods</span></span>
|<span data-ttu-id="55403-108">Метод</span><span class="sxs-lookup"><span data-stu-id="55403-108">Method</span></span>|<span data-ttu-id="55403-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55403-109">Return Type</span></span>|<span data-ttu-id="55403-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55403-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55403-111">Получение Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="55403-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="55403-112">Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="55403-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="55403-113">Чтение свойств и связей объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="55403-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="55403-114">Обновление Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="55403-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="55403-115">Девицеманажементинтентусерстатесуммари</span><span class="sxs-lookup"><span data-stu-id="55403-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="55403-116">Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="55403-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55403-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="55403-117">Properties</span></span>
|<span data-ttu-id="55403-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="55403-118">Property</span></span>|<span data-ttu-id="55403-119">Тип</span><span class="sxs-lookup"><span data-stu-id="55403-119">Type</span></span>|<span data-ttu-id="55403-120">Описание</span><span class="sxs-lookup"><span data-stu-id="55403-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55403-121">id</span><span class="sxs-lookup"><span data-stu-id="55403-121">id</span></span>|<span data-ttu-id="55403-122">String</span><span class="sxs-lookup"><span data-stu-id="55403-122">String</span></span>|<span data-ttu-id="55403-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="55403-123">The ID</span></span>|
|<span data-ttu-id="55403-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="55403-124">conflictCount</span></span>|<span data-ttu-id="55403-125">Int32</span><span class="sxs-lookup"><span data-stu-id="55403-125">Int32</span></span>|<span data-ttu-id="55403-126">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="55403-126">Number of users in conflict</span></span>|
|<span data-ttu-id="55403-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="55403-127">errorCount</span></span>|<span data-ttu-id="55403-128">Int32</span><span class="sxs-lookup"><span data-stu-id="55403-128">Int32</span></span>|<span data-ttu-id="55403-129">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="55403-129">Number of error users</span></span>|
|<span data-ttu-id="55403-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="55403-130">failedCount</span></span>|<span data-ttu-id="55403-131">Int32</span><span class="sxs-lookup"><span data-stu-id="55403-131">Int32</span></span>|<span data-ttu-id="55403-132">Количество пользователей с ошибками</span><span class="sxs-lookup"><span data-stu-id="55403-132">Number of failed users</span></span>|
|<span data-ttu-id="55403-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="55403-133">notApplicableCount</span></span>|<span data-ttu-id="55403-134">Int32</span><span class="sxs-lookup"><span data-stu-id="55403-134">Int32</span></span>|<span data-ttu-id="55403-135">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="55403-135">Number of not applicable users</span></span>|
|<span data-ttu-id="55403-136">successCount</span><span class="sxs-lookup"><span data-stu-id="55403-136">successCount</span></span>|<span data-ttu-id="55403-137">Int32</span><span class="sxs-lookup"><span data-stu-id="55403-137">Int32</span></span>|<span data-ttu-id="55403-138">Количество успешных пользователей</span><span class="sxs-lookup"><span data-stu-id="55403-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="55403-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="55403-139">Relationships</span></span>
<span data-ttu-id="55403-140">Нет</span><span class="sxs-lookup"><span data-stu-id="55403-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55403-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55403-141">JSON Representation</span></span>
<span data-ttu-id="55403-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55403-142">Here is a JSON representation of the resource.</span></span>
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







