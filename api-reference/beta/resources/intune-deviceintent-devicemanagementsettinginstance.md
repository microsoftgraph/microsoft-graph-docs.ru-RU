---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e374faf132e5da0ee3e2213e61fcdcc3078b3300
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785318"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="96912-103">Тип ресурса Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="96912-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="96912-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96912-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96912-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96912-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96912-106">Базовый тип для экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="96912-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="96912-107">Методы</span><span class="sxs-lookup"><span data-stu-id="96912-107">Methods</span></span>
|<span data-ttu-id="96912-108">Метод</span><span class="sxs-lookup"><span data-stu-id="96912-108">Method</span></span>|<span data-ttu-id="96912-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96912-109">Return Type</span></span>|<span data-ttu-id="96912-110">Описание</span><span class="sxs-lookup"><span data-stu-id="96912-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96912-111">Список Девицеманажементсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="96912-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="96912-112">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="96912-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="96912-113">Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="96912-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="96912-114">Получение Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="96912-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="96912-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="96912-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="96912-116">Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="96912-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96912-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="96912-117">Properties</span></span>
|<span data-ttu-id="96912-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="96912-118">Property</span></span>|<span data-ttu-id="96912-119">Тип</span><span class="sxs-lookup"><span data-stu-id="96912-119">Type</span></span>|<span data-ttu-id="96912-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96912-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96912-121">id</span><span class="sxs-lookup"><span data-stu-id="96912-121">id</span></span>|<span data-ttu-id="96912-122">String</span><span class="sxs-lookup"><span data-stu-id="96912-122">String</span></span>|<span data-ttu-id="96912-123">Идентификатор экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="96912-123">The setting instance ID</span></span>|
|<span data-ttu-id="96912-124">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="96912-124">definitionId</span></span>|<span data-ttu-id="96912-125">String</span><span class="sxs-lookup"><span data-stu-id="96912-125">String</span></span>|<span data-ttu-id="96912-126">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="96912-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="96912-127">валуежсон</span><span class="sxs-lookup"><span data-stu-id="96912-127">valueJson</span></span>|<span data-ttu-id="96912-128">String</span><span class="sxs-lookup"><span data-stu-id="96912-128">String</span></span>|<span data-ttu-id="96912-129">Представление значения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="96912-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="96912-130">Связи</span><span class="sxs-lookup"><span data-stu-id="96912-130">Relationships</span></span>
<span data-ttu-id="96912-131">Нет</span><span class="sxs-lookup"><span data-stu-id="96912-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96912-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96912-132">JSON Representation</span></span>
<span data-ttu-id="96912-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96912-133">Here is a JSON representation of the resource.</span></span>
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



