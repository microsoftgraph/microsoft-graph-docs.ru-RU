---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b780fad1df833a1a5d431835364493ac5afc3c6b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943335"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="76392-103">Тип ресурса Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="76392-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="76392-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76392-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76392-106">Базовый тип для экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="76392-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="76392-107">Методы</span><span class="sxs-lookup"><span data-stu-id="76392-107">Methods</span></span>
|<span data-ttu-id="76392-108">Метод</span><span class="sxs-lookup"><span data-stu-id="76392-108">Method</span></span>|<span data-ttu-id="76392-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="76392-109">Return Type</span></span>|<span data-ttu-id="76392-110">Описание</span><span class="sxs-lookup"><span data-stu-id="76392-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76392-111">Список Девицеманажементсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="76392-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="76392-112">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="76392-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="76392-113">Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="76392-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="76392-114">Получение Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="76392-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="76392-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="76392-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="76392-116">Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="76392-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76392-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="76392-117">Properties</span></span>
|<span data-ttu-id="76392-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="76392-118">Property</span></span>|<span data-ttu-id="76392-119">Тип</span><span class="sxs-lookup"><span data-stu-id="76392-119">Type</span></span>|<span data-ttu-id="76392-120">Описание</span><span class="sxs-lookup"><span data-stu-id="76392-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76392-121">id</span><span class="sxs-lookup"><span data-stu-id="76392-121">id</span></span>|<span data-ttu-id="76392-122">Строка</span><span class="sxs-lookup"><span data-stu-id="76392-122">String</span></span>|<span data-ttu-id="76392-123">Идентификатор экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="76392-123">The setting instance ID</span></span>|
|<span data-ttu-id="76392-124">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="76392-124">definitionId</span></span>|<span data-ttu-id="76392-125">Строка</span><span class="sxs-lookup"><span data-stu-id="76392-125">String</span></span>|<span data-ttu-id="76392-126">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="76392-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="76392-127">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="76392-127">valueJson</span></span>|<span data-ttu-id="76392-128">Строка</span><span class="sxs-lookup"><span data-stu-id="76392-128">String</span></span>|<span data-ttu-id="76392-129">Представление значения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="76392-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="76392-130">Связи</span><span class="sxs-lookup"><span data-stu-id="76392-130">Relationships</span></span>
<span data-ttu-id="76392-131">Нет</span><span class="sxs-lookup"><span data-stu-id="76392-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76392-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76392-132">JSON Representation</span></span>
<span data-ttu-id="76392-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76392-133">Here is a JSON representation of the resource.</span></span>
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




