---
title: Тип ресурса deviceAppManagement
description: Единичный объект управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b98aaacf4af9b646bb25f4131150d613e2336a87
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757591"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="7416c-103">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7416c-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="7416c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7416c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7416c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7416c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7416c-106">Единичный объект управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="7416c-106">Device app management singleton entity.</span></span>

## <a name="methods"></a><span data-ttu-id="7416c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7416c-107">Methods</span></span>
|<span data-ttu-id="7416c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7416c-108">Method</span></span>|<span data-ttu-id="7416c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7416c-109">Return Type</span></span>|<span data-ttu-id="7416c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7416c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7416c-111">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7416c-111">Get deviceAppManagement</span></span>](../api/intune-partnerintegration-deviceappmanagement-get.md)|[<span data-ttu-id="7416c-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7416c-112">deviceAppManagement</span></span>](../resources/intune-partnerintegration-deviceappmanagement.md)|<span data-ttu-id="7416c-113">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7416c-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="7416c-114">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7416c-114">Update deviceAppManagement</span></span>](../api/intune-partnerintegration-deviceappmanagement-update.md)|[<span data-ttu-id="7416c-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="7416c-115">deviceAppManagement</span></span>](../resources/intune-partnerintegration-deviceappmanagement.md)|<span data-ttu-id="7416c-116">Обновление свойств объекта [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7416c-116">Update the properties of a [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7416c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7416c-117">Properties</span></span>
|<span data-ttu-id="7416c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7416c-118">Property</span></span>|<span data-ttu-id="7416c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7416c-119">Type</span></span>|<span data-ttu-id="7416c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7416c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7416c-121">id</span><span class="sxs-lookup"><span data-stu-id="7416c-121">id</span></span>|<span data-ttu-id="7416c-122">String</span><span class="sxs-lookup"><span data-stu-id="7416c-122">String</span></span>|<span data-ttu-id="7416c-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7416c-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7416c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="7416c-124">Relationships</span></span>
<span data-ttu-id="7416c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7416c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7416c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7416c-126">JSON Representation</span></span>
<span data-ttu-id="7416c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7416c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




