---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d0a20bc936a4fd3e4c83ad65a237d341dd4fd39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752013"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="1cf19-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1cf19-103">deviceManagement resource type</span></span>

<span data-ttu-id="1cf19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cf19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cf19-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cf19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cf19-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1cf19-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="1cf19-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1cf19-107">Methods</span></span>
|<span data-ttu-id="1cf19-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1cf19-108">Method</span></span>|<span data-ttu-id="1cf19-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1cf19-109">Return Type</span></span>|<span data-ttu-id="1cf19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf19-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1cf19-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1cf19-111">Get deviceManagement</span></span>](../api/intune-remoteassistance-devicemanagement-get.md)|[<span data-ttu-id="1cf19-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1cf19-112">deviceManagement</span></span>](../resources/intune-remoteassistance-devicemanagement.md)|<span data-ttu-id="1cf19-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1cf19-113">Read properties and relationships of the [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="1cf19-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1cf19-114">Update deviceManagement</span></span>](../api/intune-remoteassistance-devicemanagement-update.md)|[<span data-ttu-id="1cf19-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1cf19-115">deviceManagement</span></span>](../resources/intune-remoteassistance-devicemanagement.md)|<span data-ttu-id="1cf19-116">Обновление свойств объекта [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1cf19-116">Update the properties of a [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1cf19-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cf19-117">Properties</span></span>
|<span data-ttu-id="1cf19-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cf19-118">Property</span></span>|<span data-ttu-id="1cf19-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf19-119">Type</span></span>|<span data-ttu-id="1cf19-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf19-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cf19-121">id</span><span class="sxs-lookup"><span data-stu-id="1cf19-121">id</span></span>|<span data-ttu-id="1cf19-122">String</span><span class="sxs-lookup"><span data-stu-id="1cf19-122">String</span></span>|<span data-ttu-id="1cf19-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1cf19-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cf19-124">Связи</span><span class="sxs-lookup"><span data-stu-id="1cf19-124">Relationships</span></span>
|<span data-ttu-id="1cf19-125">Связь</span><span class="sxs-lookup"><span data-stu-id="1cf19-125">Relationship</span></span>|<span data-ttu-id="1cf19-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf19-126">Type</span></span>|<span data-ttu-id="1cf19-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf19-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cf19-128">remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="1cf19-128">remoteAssistancePartners</span></span>|<span data-ttu-id="1cf19-129">Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)</span><span class="sxs-lookup"><span data-stu-id="1cf19-129">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="1cf19-130">Партнеры по удаленной помощи.</span><span class="sxs-lookup"><span data-stu-id="1cf19-130">The remote assist partners.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cf19-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cf19-131">JSON Representation</span></span>
<span data-ttu-id="1cf19-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cf19-132">Here is a JSON representation of the resource.</span></span>
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




