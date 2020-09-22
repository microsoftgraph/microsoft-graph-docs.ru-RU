---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a035fcb23b3137bfe4e278e12d71a754d1e69d05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061184"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="28a44-103">Тип ресурса Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="28a44-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="28a44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28a44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28a44-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28a44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28a44-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28a44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a44-107">Базовый тип для экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="28a44-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="28a44-108">Методы</span><span class="sxs-lookup"><span data-stu-id="28a44-108">Methods</span></span>
|<span data-ttu-id="28a44-109">Метод</span><span class="sxs-lookup"><span data-stu-id="28a44-109">Method</span></span>|<span data-ttu-id="28a44-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28a44-110">Return Type</span></span>|<span data-ttu-id="28a44-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28a44-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28a44-112">Список Девицеманажементсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="28a44-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="28a44-113">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="28a44-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="28a44-114">Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="28a44-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="28a44-115">Получение Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="28a44-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="28a44-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="28a44-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="28a44-117">Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="28a44-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28a44-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="28a44-118">Properties</span></span>
|<span data-ttu-id="28a44-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="28a44-119">Property</span></span>|<span data-ttu-id="28a44-120">Тип</span><span class="sxs-lookup"><span data-stu-id="28a44-120">Type</span></span>|<span data-ttu-id="28a44-121">Описание</span><span class="sxs-lookup"><span data-stu-id="28a44-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a44-122">id</span><span class="sxs-lookup"><span data-stu-id="28a44-122">id</span></span>|<span data-ttu-id="28a44-123">String</span><span class="sxs-lookup"><span data-stu-id="28a44-123">String</span></span>|<span data-ttu-id="28a44-124">Идентификатор экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="28a44-124">The setting instance ID</span></span>|
|<span data-ttu-id="28a44-125">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="28a44-125">definitionId</span></span>|<span data-ttu-id="28a44-126">String</span><span class="sxs-lookup"><span data-stu-id="28a44-126">String</span></span>|<span data-ttu-id="28a44-127">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="28a44-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="28a44-128">валуежсон</span><span class="sxs-lookup"><span data-stu-id="28a44-128">valueJson</span></span>|<span data-ttu-id="28a44-129">String</span><span class="sxs-lookup"><span data-stu-id="28a44-129">String</span></span>|<span data-ttu-id="28a44-130">Представление значения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="28a44-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="28a44-131">Связи</span><span class="sxs-lookup"><span data-stu-id="28a44-131">Relationships</span></span>
<span data-ttu-id="28a44-132">Нет</span><span class="sxs-lookup"><span data-stu-id="28a44-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28a44-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28a44-133">JSON Representation</span></span>
<span data-ttu-id="28a44-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28a44-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```






