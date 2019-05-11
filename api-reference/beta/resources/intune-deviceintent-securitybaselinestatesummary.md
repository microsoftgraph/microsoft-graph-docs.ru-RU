---
title: Тип ресурса Секуритибаселинестатесуммари
description: Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c7c1cf31ddca02348eed55b9dc19dd5420b016e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943272"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="cd5aa-103">Тип ресурса Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="cd5aa-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="cd5aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd5aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd5aa-106">Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="cd5aa-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cd5aa-107">Methods</span></span>
|<span data-ttu-id="cd5aa-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cd5aa-108">Method</span></span>|<span data-ttu-id="cd5aa-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd5aa-109">Return Type</span></span>|<span data-ttu-id="cd5aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd5aa-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd5aa-111">Получение Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="cd5aa-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="cd5aa-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="cd5aa-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="cd5aa-113">Чтение свойств и связей объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cd5aa-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="cd5aa-114">Обновление Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="cd5aa-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="cd5aa-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="cd5aa-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="cd5aa-116">Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cd5aa-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd5aa-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd5aa-117">Properties</span></span>
|<span data-ttu-id="cd5aa-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd5aa-118">Property</span></span>|<span data-ttu-id="cd5aa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cd5aa-119">Type</span></span>|<span data-ttu-id="cd5aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cd5aa-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd5aa-121">id</span><span class="sxs-lookup"><span data-stu-id="cd5aa-121">id</span></span>|<span data-ttu-id="cd5aa-122">Строка</span><span class="sxs-lookup"><span data-stu-id="cd5aa-122">String</span></span>|<span data-ttu-id="cd5aa-123">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="cd5aa-124">Секурекаунт</span><span class="sxs-lookup"><span data-stu-id="cd5aa-124">secureCount</span></span>|<span data-ttu-id="cd5aa-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cd5aa-125">Int32</span></span>|<span data-ttu-id="cd5aa-126">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="cd5aa-126">Number of secure devices</span></span>|
|<span data-ttu-id="cd5aa-127">Нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="cd5aa-127">notSecureCount</span></span>|<span data-ttu-id="cd5aa-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cd5aa-128">Int32</span></span>|<span data-ttu-id="cd5aa-129">Количество незащищенных устройств</span><span class="sxs-lookup"><span data-stu-id="cd5aa-129">Number of not secure devices</span></span>|
|<span data-ttu-id="cd5aa-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="cd5aa-130">unknownCount</span></span>|<span data-ttu-id="cd5aa-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cd5aa-131">Int32</span></span>|<span data-ttu-id="cd5aa-132">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-132">Number of unknown devices</span></span>|
|<span data-ttu-id="cd5aa-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="cd5aa-133">errorCount</span></span>|<span data-ttu-id="cd5aa-134">Int32</span><span class="sxs-lookup"><span data-stu-id="cd5aa-134">Int32</span></span>|<span data-ttu-id="cd5aa-135">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-135">Number of error devices</span></span>|
|<span data-ttu-id="cd5aa-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="cd5aa-136">conflictCount</span></span>|<span data-ttu-id="cd5aa-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cd5aa-137">Int32</span></span>|<span data-ttu-id="cd5aa-138">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-138">Number of conflict devices</span></span>|
|<span data-ttu-id="cd5aa-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cd5aa-139">notApplicableCount</span></span>|<span data-ttu-id="cd5aa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cd5aa-140">Int32</span></span>|<span data-ttu-id="cd5aa-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd5aa-142">Связи</span><span class="sxs-lookup"><span data-stu-id="cd5aa-142">Relationships</span></span>
<span data-ttu-id="cd5aa-143">Нет</span><span class="sxs-lookup"><span data-stu-id="cd5aa-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd5aa-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd5aa-144">JSON Representation</span></span>
<span data-ttu-id="cd5aa-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd5aa-145">Here is a JSON representation of the resource.</span></span>
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




