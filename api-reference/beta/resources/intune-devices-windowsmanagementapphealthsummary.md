---
title: Тип ресурса Виндовсманажементапфеалссуммари
description: Содержит свойства для сводки о работоспособности приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aea7f113d144ca876b301acc3b303ac0f7072bc4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520027"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="05718-103">Тип ресурса Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="05718-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="05718-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05718-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05718-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05718-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05718-106">Содержит свойства для сводки о работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="05718-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="05718-107">Методы</span><span class="sxs-lookup"><span data-stu-id="05718-107">Methods</span></span>
|<span data-ttu-id="05718-108">Метод</span><span class="sxs-lookup"><span data-stu-id="05718-108">Method</span></span>|<span data-ttu-id="05718-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05718-109">Return Type</span></span>|<span data-ttu-id="05718-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05718-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05718-111">Получение Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="05718-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|<span data-ttu-id="05718-112">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05718-112">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="05718-113">Чтение свойств и связей объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="05718-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="05718-114">Обновление Виндовсманажементапфеалссуммари</span><span class="sxs-lookup"><span data-stu-id="05718-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|<span data-ttu-id="05718-115">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="05718-115">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="05718-116">Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="05718-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05718-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="05718-117">Properties</span></span>
|<span data-ttu-id="05718-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="05718-118">Property</span></span>|<span data-ttu-id="05718-119">Тип</span><span class="sxs-lookup"><span data-stu-id="05718-119">Type</span></span>|<span data-ttu-id="05718-120">Описание</span><span class="sxs-lookup"><span data-stu-id="05718-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05718-121">id</span><span class="sxs-lookup"><span data-stu-id="05718-121">id</span></span>|<span data-ttu-id="05718-122">String</span><span class="sxs-lookup"><span data-stu-id="05718-122">String</span></span>|<span data-ttu-id="05718-123">Ключ объекта сводки работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="05718-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="05718-124">Хеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="05718-124">healthyDeviceCount</span></span>|<span data-ttu-id="05718-125">Int32</span><span class="sxs-lookup"><span data-stu-id="05718-125">Int32</span></span>|<span data-ttu-id="05718-126">Работоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="05718-126">Healthy device count.</span></span>|
|<span data-ttu-id="05718-127">Унхеалсидевицекаунт</span><span class="sxs-lookup"><span data-stu-id="05718-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="05718-128">Int32</span><span class="sxs-lookup"><span data-stu-id="05718-128">Int32</span></span>|<span data-ttu-id="05718-129">Неработоспособное число устройств.</span><span class="sxs-lookup"><span data-stu-id="05718-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="05718-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05718-130">unknownDeviceCount</span></span>|<span data-ttu-id="05718-131">Int32</span><span class="sxs-lookup"><span data-stu-id="05718-131">Int32</span></span>|<span data-ttu-id="05718-132">Количество неИзвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="05718-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05718-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="05718-133">Relationships</span></span>
<span data-ttu-id="05718-134">Нет</span><span class="sxs-lookup"><span data-stu-id="05718-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05718-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05718-135">JSON Representation</span></span>
<span data-ttu-id="05718-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05718-136">Here is a JSON representation of the resource.</span></span>
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





