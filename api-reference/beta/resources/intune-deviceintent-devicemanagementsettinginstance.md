---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49f97d47b5ff75e927a5637356476392047a2f8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550541"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="686a2-103">Тип ресурса Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="686a2-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="686a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="686a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="686a2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="686a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="686a2-106">Базовый тип для экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="686a2-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="686a2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="686a2-107">Methods</span></span>
|<span data-ttu-id="686a2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="686a2-108">Method</span></span>|<span data-ttu-id="686a2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="686a2-109">Return Type</span></span>|<span data-ttu-id="686a2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="686a2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="686a2-111">Список Девицеманажементсеттингинстанцес</span><span class="sxs-lookup"><span data-stu-id="686a2-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="686a2-112">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="686a2-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="686a2-113">Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="686a2-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="686a2-114">Получение Девицеманажементсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="686a2-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="686a2-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="686a2-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="686a2-116">Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="686a2-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="686a2-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="686a2-117">Properties</span></span>
|<span data-ttu-id="686a2-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="686a2-118">Property</span></span>|<span data-ttu-id="686a2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="686a2-119">Type</span></span>|<span data-ttu-id="686a2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="686a2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="686a2-121">id</span><span class="sxs-lookup"><span data-stu-id="686a2-121">id</span></span>|<span data-ttu-id="686a2-122">String</span><span class="sxs-lookup"><span data-stu-id="686a2-122">String</span></span>|<span data-ttu-id="686a2-123">Идентификатор экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="686a2-123">The setting instance ID</span></span>|
|<span data-ttu-id="686a2-124">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="686a2-124">definitionId</span></span>|<span data-ttu-id="686a2-125">String</span><span class="sxs-lookup"><span data-stu-id="686a2-125">String</span></span>|<span data-ttu-id="686a2-126">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="686a2-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="686a2-127">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="686a2-127">valueJson</span></span>|<span data-ttu-id="686a2-128">String</span><span class="sxs-lookup"><span data-stu-id="686a2-128">String</span></span>|<span data-ttu-id="686a2-129">Представление значения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="686a2-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="686a2-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="686a2-130">Relationships</span></span>
<span data-ttu-id="686a2-131">Нет</span><span class="sxs-lookup"><span data-stu-id="686a2-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="686a2-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="686a2-132">JSON Representation</span></span>
<span data-ttu-id="686a2-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="686a2-133">Here is a JSON representation of the resource.</span></span>
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





