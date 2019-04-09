---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9aef844dd4957b75b51f8d16014c2253b0253cc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523611"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="efdcd-103">Тип ресурса Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="efdcd-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="efdcd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efdcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efdcd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efdcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efdcd-106">Базовый тип для экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="efdcd-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="efdcd-107">Методы</span><span class="sxs-lookup"><span data-stu-id="efdcd-107">Methods</span></span>
|<span data-ttu-id="efdcd-108">Метод</span><span class="sxs-lookup"><span data-stu-id="efdcd-108">Method</span></span>|<span data-ttu-id="efdcd-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efdcd-109">Return Type</span></span>|<span data-ttu-id="efdcd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="efdcd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="efdcd-111">Список Девицеманажементсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="efdcd-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="efdcd-112">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="efdcd-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="efdcd-113">Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="efdcd-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="efdcd-114">Получение Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="efdcd-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="efdcd-115">Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="efdcd-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="efdcd-116">Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="efdcd-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="efdcd-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="efdcd-117">Properties</span></span>
|<span data-ttu-id="efdcd-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="efdcd-118">Property</span></span>|<span data-ttu-id="efdcd-119">Тип</span><span class="sxs-lookup"><span data-stu-id="efdcd-119">Type</span></span>|<span data-ttu-id="efdcd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="efdcd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efdcd-121">id</span><span class="sxs-lookup"><span data-stu-id="efdcd-121">id</span></span>|<span data-ttu-id="efdcd-122">String</span><span class="sxs-lookup"><span data-stu-id="efdcd-122">String</span></span>|<span data-ttu-id="efdcd-123">Идентификатор экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="efdcd-123">The setting instance ID</span></span>|
|<span data-ttu-id="efdcd-124">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="efdcd-124">definitionId</span></span>|<span data-ttu-id="efdcd-125">String</span><span class="sxs-lookup"><span data-stu-id="efdcd-125">String</span></span>|<span data-ttu-id="efdcd-126">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="efdcd-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="efdcd-127">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="efdcd-127">valueJson</span></span>|<span data-ttu-id="efdcd-128">String</span><span class="sxs-lookup"><span data-stu-id="efdcd-128">String</span></span>|<span data-ttu-id="efdcd-129">Представление значения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="efdcd-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="efdcd-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="efdcd-130">Relationships</span></span>
<span data-ttu-id="efdcd-131">Нет</span><span class="sxs-lookup"><span data-stu-id="efdcd-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efdcd-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efdcd-132">JSON Representation</span></span>
<span data-ttu-id="efdcd-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efdcd-133">Here is a JSON representation of the resource.</span></span>
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







