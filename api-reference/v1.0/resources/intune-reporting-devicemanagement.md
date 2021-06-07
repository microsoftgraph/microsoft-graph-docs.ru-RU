---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76e65eb3d4d49644d8f6350ad838b53c5990eee5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753116"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="a4c48-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a4c48-103">deviceManagement resource type</span></span>

<span data-ttu-id="a4c48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4c48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4c48-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4c48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4c48-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="a4c48-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="a4c48-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a4c48-107">Methods</span></span>
|<span data-ttu-id="a4c48-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a4c48-108">Method</span></span>|<span data-ttu-id="a4c48-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4c48-109">Return Type</span></span>|<span data-ttu-id="a4c48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a4c48-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a4c48-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a4c48-111">Get deviceManagement</span></span>](../api/intune-reporting-devicemanagement-get.md)|[<span data-ttu-id="a4c48-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a4c48-112">deviceManagement</span></span>](../resources/intune-reporting-devicemanagement.md)|<span data-ttu-id="a4c48-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-reporting-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a4c48-113">Read properties and relationships of the [deviceManagement](../resources/intune-reporting-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="a4c48-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a4c48-114">Update deviceManagement</span></span>](../api/intune-reporting-devicemanagement-update.md)|[<span data-ttu-id="a4c48-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a4c48-115">deviceManagement</span></span>](../resources/intune-reporting-devicemanagement.md)|<span data-ttu-id="a4c48-116">Обновление свойств объекта [deviceManagement](../resources/intune-reporting-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a4c48-116">Update the properties of a [deviceManagement](../resources/intune-reporting-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4c48-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4c48-117">Properties</span></span>
|<span data-ttu-id="a4c48-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4c48-118">Property</span></span>|<span data-ttu-id="a4c48-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a4c48-119">Type</span></span>|<span data-ttu-id="a4c48-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4c48-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c48-121">id</span><span class="sxs-lookup"><span data-stu-id="a4c48-121">id</span></span>|<span data-ttu-id="a4c48-122">String</span><span class="sxs-lookup"><span data-stu-id="a4c48-122">String</span></span>|<span data-ttu-id="a4c48-123">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="a4c48-123">Unique identifier for this entity</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4c48-124">Связи</span><span class="sxs-lookup"><span data-stu-id="a4c48-124">Relationships</span></span>
|<span data-ttu-id="a4c48-125">Связь</span><span class="sxs-lookup"><span data-stu-id="a4c48-125">Relationship</span></span>|<span data-ttu-id="a4c48-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a4c48-126">Type</span></span>|<span data-ttu-id="a4c48-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a4c48-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c48-128">отчеты</span><span class="sxs-lookup"><span data-stu-id="a4c48-128">reports</span></span>|[<span data-ttu-id="a4c48-129">deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="a4c48-129">deviceManagementReports</span></span>](../resources/intune-reporting-devicemanagementreports.md)|<span data-ttu-id="a4c48-130">Отчеты singleton</span><span class="sxs-lookup"><span data-stu-id="a4c48-130">Reports singleton</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4c48-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4c48-131">JSON Representation</span></span>
<span data-ttu-id="a4c48-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4c48-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




