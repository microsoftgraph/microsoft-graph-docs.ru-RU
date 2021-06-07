---
title: Тип ресурса deviceManagement
description: Ресурс deviceManagement представляет идентификаторы устройств из коллекции клиента, которые были предварительно подготовлены в Intune, и профили регистрации, которые можно назначать идентификаторам устройств, поддерживающим конфигурацию до регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38c93be6c71f97e828901f51c7d6851a346f0bd1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755427"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="2f305-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f305-103">deviceManagement resource type</span></span>

<span data-ttu-id="2f305-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f305-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f305-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f305-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f305-106">Ресурс deviceManagement представляет идентификаторы устройств из коллекции клиента, которые были предварительно подготовлены в Intune, и профили регистрации, которые можно назначать идентификаторам устройств, поддерживающим конфигурацию до регистрации.</span><span class="sxs-lookup"><span data-stu-id="2f305-106">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="2f305-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2f305-107">Methods</span></span>
|<span data-ttu-id="2f305-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2f305-108">Method</span></span>|<span data-ttu-id="2f305-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f305-109">Return Type</span></span>|<span data-ttu-id="2f305-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f305-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f305-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f305-111">Get deviceManagement</span></span>](../api/intune-enrollment-devicemanagement-get.md)|[<span data-ttu-id="2f305-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f305-112">deviceManagement</span></span>](../resources/intune-enrollment-devicemanagement.md)|<span data-ttu-id="2f305-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-enrollment-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2f305-113">Read properties and relationships of the [deviceManagement](../resources/intune-enrollment-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="2f305-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f305-114">Update deviceManagement</span></span>](../api/intune-enrollment-devicemanagement-update.md)|[<span data-ttu-id="2f305-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f305-115">deviceManagement</span></span>](../resources/intune-enrollment-devicemanagement.md)|<span data-ttu-id="2f305-116">Обновление свойств объекта [deviceManagement](../resources/intune-enrollment-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2f305-116">Update the properties of a [deviceManagement](../resources/intune-enrollment-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f305-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f305-117">Properties</span></span>
|<span data-ttu-id="2f305-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f305-118">Property</span></span>|<span data-ttu-id="2f305-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2f305-119">Type</span></span>|<span data-ttu-id="2f305-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2f305-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f305-121">id</span><span class="sxs-lookup"><span data-stu-id="2f305-121">id</span></span>|<span data-ttu-id="2f305-122">String</span><span class="sxs-lookup"><span data-stu-id="2f305-122">String</span></span>|<span data-ttu-id="2f305-123">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="2f305-123">The GUID for the object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f305-124">Связи</span><span class="sxs-lookup"><span data-stu-id="2f305-124">Relationships</span></span>
|<span data-ttu-id="2f305-125">Связь</span><span class="sxs-lookup"><span data-stu-id="2f305-125">Relationship</span></span>|<span data-ttu-id="2f305-126">Тип</span><span class="sxs-lookup"><span data-stu-id="2f305-126">Type</span></span>|<span data-ttu-id="2f305-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2f305-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f305-128">windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2f305-128">windowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="2f305-129">[коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2f305-129">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="2f305-130">Идентификаторы Windows автопилота содержали коллекцию.</span><span class="sxs-lookup"><span data-stu-id="2f305-130">The Windows autopilot device identities contained collection.</span></span>|
|<span data-ttu-id="2f305-131">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2f305-131">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="2f305-132">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2f305-132">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="2f305-133">Коллекция импортированных устройств Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2f305-133">Collection of imported Windows autopilot devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f305-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f305-134">JSON Representation</span></span>
<span data-ttu-id="2f305-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f305-135">Here is a JSON representation of the resource.</span></span>
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




