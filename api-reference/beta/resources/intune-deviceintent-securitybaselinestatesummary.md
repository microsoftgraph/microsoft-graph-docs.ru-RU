---
title: Тип ресурса Секуритибаселинестатесуммари
description: Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8133fb325b0c2abdacf38e034aedc6523b13623c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562225"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="b0396-103">Тип ресурса Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="b0396-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="b0396-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0396-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0396-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0396-106">Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b0396-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="b0396-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b0396-107">Methods</span></span>
|<span data-ttu-id="b0396-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b0396-108">Method</span></span>|<span data-ttu-id="b0396-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b0396-109">Return Type</span></span>|<span data-ttu-id="b0396-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0396-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0396-111">Получение Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="b0396-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="b0396-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="b0396-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="b0396-113">Чтение свойств и связей объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b0396-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="b0396-114">Обновление Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="b0396-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="b0396-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="b0396-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="b0396-116">Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b0396-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0396-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0396-117">Properties</span></span>
|<span data-ttu-id="b0396-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0396-118">Property</span></span>|<span data-ttu-id="b0396-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b0396-119">Type</span></span>|<span data-ttu-id="b0396-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b0396-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0396-121">id</span><span class="sxs-lookup"><span data-stu-id="b0396-121">id</span></span>|<span data-ttu-id="b0396-122">String</span><span class="sxs-lookup"><span data-stu-id="b0396-122">String</span></span>|<span data-ttu-id="b0396-123">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b0396-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b0396-124">Секурекаунт</span><span class="sxs-lookup"><span data-stu-id="b0396-124">secureCount</span></span>|<span data-ttu-id="b0396-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b0396-125">Int32</span></span>|<span data-ttu-id="b0396-126">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="b0396-126">Number of secure devices</span></span>|
|<span data-ttu-id="b0396-127">Нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="b0396-127">notSecureCount</span></span>|<span data-ttu-id="b0396-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b0396-128">Int32</span></span>|<span data-ttu-id="b0396-129">Количество незащищенных устройств</span><span class="sxs-lookup"><span data-stu-id="b0396-129">Number of not secure devices</span></span>|
|<span data-ttu-id="b0396-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="b0396-130">unknownCount</span></span>|<span data-ttu-id="b0396-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b0396-131">Int32</span></span>|<span data-ttu-id="b0396-132">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="b0396-132">Number of unknown devices</span></span>|
|<span data-ttu-id="b0396-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="b0396-133">errorCount</span></span>|<span data-ttu-id="b0396-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b0396-134">Int32</span></span>|<span data-ttu-id="b0396-135">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b0396-135">Number of error devices</span></span>|
|<span data-ttu-id="b0396-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b0396-136">conflictCount</span></span>|<span data-ttu-id="b0396-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b0396-137">Int32</span></span>|<span data-ttu-id="b0396-138">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="b0396-138">Number of conflict devices</span></span>|
|<span data-ttu-id="b0396-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b0396-139">notApplicableCount</span></span>|<span data-ttu-id="b0396-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b0396-140">Int32</span></span>|<span data-ttu-id="b0396-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="b0396-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0396-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0396-142">Relationships</span></span>
<span data-ttu-id="b0396-143">Нет</span><span class="sxs-lookup"><span data-stu-id="b0396-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0396-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0396-144">JSON Representation</span></span>
<span data-ttu-id="b0396-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0396-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```





