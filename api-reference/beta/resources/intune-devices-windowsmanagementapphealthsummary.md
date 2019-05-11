---
title: Тип ресурса Виндовсманажементапфеалссуммари
description: Содержит свойства для сводки о работоспособности приложения управления Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07e782cb14ab2ee4996ff8e53f61323693e00846
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941690"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="c63cc-103">Тип ресурса Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="c63cc-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="c63cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c63cc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c63cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63cc-106">Содержит свойства для сводки о работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="c63cc-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="c63cc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c63cc-107">Methods</span></span>
|<span data-ttu-id="c63cc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c63cc-108">Method</span></span>|<span data-ttu-id="c63cc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c63cc-109">Return Type</span></span>|<span data-ttu-id="c63cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c63cc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c63cc-111">Получение Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="c63cc-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|<span data-ttu-id="c63cc-112">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c63cc-112">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="c63cc-113">Чтение свойств и связей объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c63cc-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="c63cc-114">Обновление Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="c63cc-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|<span data-ttu-id="c63cc-115">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c63cc-115">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="c63cc-116">Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c63cc-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c63cc-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c63cc-117">Properties</span></span>
|<span data-ttu-id="c63cc-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c63cc-118">Property</span></span>|<span data-ttu-id="c63cc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c63cc-119">Type</span></span>|<span data-ttu-id="c63cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c63cc-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63cc-121">id</span><span class="sxs-lookup"><span data-stu-id="c63cc-121">id</span></span>|<span data-ttu-id="c63cc-122">Строка</span><span class="sxs-lookup"><span data-stu-id="c63cc-122">String</span></span>|<span data-ttu-id="c63cc-123">Ключ объекта сводки работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="c63cc-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="c63cc-124">Хеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c63cc-124">healthyDeviceCount</span></span>|<span data-ttu-id="c63cc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c63cc-125">Int32</span></span>|<span data-ttu-id="c63cc-126">Работоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="c63cc-126">Healthy device count.</span></span>|
|<span data-ttu-id="c63cc-127">Унхеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c63cc-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="c63cc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c63cc-128">Int32</span></span>|<span data-ttu-id="c63cc-129">Неработоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="c63cc-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="c63cc-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c63cc-130">unknownDeviceCount</span></span>|<span data-ttu-id="c63cc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c63cc-131">Int32</span></span>|<span data-ttu-id="c63cc-132">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="c63cc-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c63cc-133">Связи</span><span class="sxs-lookup"><span data-stu-id="c63cc-133">Relationships</span></span>
<span data-ttu-id="c63cc-134">Нет</span><span class="sxs-lookup"><span data-stu-id="c63cc-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c63cc-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c63cc-135">JSON Representation</span></span>
<span data-ttu-id="c63cc-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c63cc-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




