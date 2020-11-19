---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 882dae54c63dabc70e320f9965eaefe693b05f4e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268052"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="6a24b-103">Тип ресурса Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="6a24b-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="6a24b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a24b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a24b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a24b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a24b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a24b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a24b-107">Базовый тип для экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="6a24b-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="6a24b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6a24b-108">Methods</span></span>
|<span data-ttu-id="6a24b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6a24b-109">Method</span></span>|<span data-ttu-id="6a24b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6a24b-110">Return Type</span></span>|<span data-ttu-id="6a24b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a24b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a24b-112">Список Девицеманажементсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="6a24b-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="6a24b-113">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="6a24b-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="6a24b-114">Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="6a24b-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="6a24b-115">Получение Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="6a24b-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="6a24b-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="6a24b-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="6a24b-117">Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="6a24b-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a24b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a24b-118">Properties</span></span>
|<span data-ttu-id="6a24b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a24b-119">Property</span></span>|<span data-ttu-id="6a24b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6a24b-120">Type</span></span>|<span data-ttu-id="6a24b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6a24b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a24b-122">id</span><span class="sxs-lookup"><span data-stu-id="6a24b-122">id</span></span>|<span data-ttu-id="6a24b-123">String</span><span class="sxs-lookup"><span data-stu-id="6a24b-123">String</span></span>|<span data-ttu-id="6a24b-124">Идентификатор экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="6a24b-124">The setting instance ID</span></span>|
|<span data-ttu-id="6a24b-125">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="6a24b-125">definitionId</span></span>|<span data-ttu-id="6a24b-126">String</span><span class="sxs-lookup"><span data-stu-id="6a24b-126">String</span></span>|<span data-ttu-id="6a24b-127">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="6a24b-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="6a24b-128">валуежсон</span><span class="sxs-lookup"><span data-stu-id="6a24b-128">valueJson</span></span>|<span data-ttu-id="6a24b-129">String</span><span class="sxs-lookup"><span data-stu-id="6a24b-129">String</span></span>|<span data-ttu-id="6a24b-130">Представление значения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6a24b-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a24b-131">Связи</span><span class="sxs-lookup"><span data-stu-id="6a24b-131">Relationships</span></span>
<span data-ttu-id="6a24b-132">Нет</span><span class="sxs-lookup"><span data-stu-id="6a24b-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a24b-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a24b-133">JSON Representation</span></span>
<span data-ttu-id="6a24b-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a24b-134">Here is a JSON representation of the resource.</span></span>
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




