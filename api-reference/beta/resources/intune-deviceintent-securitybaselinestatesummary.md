---
title: Тип ресурса Секуритибаселинестатесуммари
description: Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f162da0276f9759fa04f40cbd99a57ac6816b5bc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209243"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="7395c-103">Тип ресурса Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="7395c-103">securityBaselineStateSummary resource type</span></span>

<span data-ttu-id="7395c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7395c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7395c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7395c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7395c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7395c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7395c-107">Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7395c-107">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="7395c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7395c-108">Methods</span></span>
|<span data-ttu-id="7395c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7395c-109">Method</span></span>|<span data-ttu-id="7395c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7395c-110">Return Type</span></span>|<span data-ttu-id="7395c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7395c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7395c-112">Получение Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="7395c-112">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="7395c-113">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7395c-113">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="7395c-114">Чтение свойств и связей объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7395c-114">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="7395c-115">Обновление Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="7395c-115">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="7395c-116">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7395c-116">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="7395c-117">Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7395c-117">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7395c-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="7395c-118">Properties</span></span>
|<span data-ttu-id="7395c-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="7395c-119">Property</span></span>|<span data-ttu-id="7395c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7395c-120">Type</span></span>|<span data-ttu-id="7395c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7395c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7395c-122">id</span><span class="sxs-lookup"><span data-stu-id="7395c-122">id</span></span>|<span data-ttu-id="7395c-123">String</span><span class="sxs-lookup"><span data-stu-id="7395c-123">String</span></span>|<span data-ttu-id="7395c-124">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7395c-124">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7395c-125">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="7395c-125">secureCount</span></span>|<span data-ttu-id="7395c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="7395c-126">Int32</span></span>|<span data-ttu-id="7395c-127">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="7395c-127">Number of secure devices</span></span>|
|<span data-ttu-id="7395c-128">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="7395c-128">notSecureCount</span></span>|<span data-ttu-id="7395c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="7395c-129">Int32</span></span>|<span data-ttu-id="7395c-130">Количество незащищенных устройств</span><span class="sxs-lookup"><span data-stu-id="7395c-130">Number of not secure devices</span></span>|
|<span data-ttu-id="7395c-131">unknownCount</span><span class="sxs-lookup"><span data-stu-id="7395c-131">unknownCount</span></span>|<span data-ttu-id="7395c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7395c-132">Int32</span></span>|<span data-ttu-id="7395c-133">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="7395c-133">Number of unknown devices</span></span>|
|<span data-ttu-id="7395c-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="7395c-134">errorCount</span></span>|<span data-ttu-id="7395c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7395c-135">Int32</span></span>|<span data-ttu-id="7395c-136">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7395c-136">Number of error devices</span></span>|
|<span data-ttu-id="7395c-137">conflictCount</span><span class="sxs-lookup"><span data-stu-id="7395c-137">conflictCount</span></span>|<span data-ttu-id="7395c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7395c-138">Int32</span></span>|<span data-ttu-id="7395c-139">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="7395c-139">Number of conflict devices</span></span>|
|<span data-ttu-id="7395c-140">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7395c-140">notApplicableCount</span></span>|<span data-ttu-id="7395c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7395c-141">Int32</span></span>|<span data-ttu-id="7395c-142">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="7395c-142">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="7395c-143">Связи</span><span class="sxs-lookup"><span data-stu-id="7395c-143">Relationships</span></span>
<span data-ttu-id="7395c-144">Нет</span><span class="sxs-lookup"><span data-stu-id="7395c-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7395c-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7395c-145">JSON Representation</span></span>
<span data-ttu-id="7395c-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7395c-146">Here is a JSON representation of the resource.</span></span>
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




