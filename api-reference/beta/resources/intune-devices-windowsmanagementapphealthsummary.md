---
title: Тип ресурса windowsManagementAppHealthSummary
description: Содержит свойства для Сводка работоспособности приложения управления Windows.
ms.openlocfilehash: dddcb40a0a66446ab6e87a2e684c1dbf0df547fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078446"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="638bc-103">Тип ресурса windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="638bc-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="638bc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="638bc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="638bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="638bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="638bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="638bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="638bc-107">Содержит свойства для Сводка работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="638bc-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="638bc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="638bc-108">Methods</span></span>
|<span data-ttu-id="638bc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="638bc-109">Method</span></span>|<span data-ttu-id="638bc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="638bc-110">Return Type</span></span>|<span data-ttu-id="638bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="638bc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="638bc-112">Получение windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="638bc-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|<span data-ttu-id="638bc-113">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="638bc-113">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="638bc-114">Чтение свойства и связи объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="638bc-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="638bc-115">Обновление windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="638bc-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|<span data-ttu-id="638bc-116">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="638bc-116">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="638bc-117">Обновление свойства объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="638bc-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="638bc-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="638bc-118">Properties</span></span>
|<span data-ttu-id="638bc-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="638bc-119">Property</span></span>|<span data-ttu-id="638bc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="638bc-120">Type</span></span>|<span data-ttu-id="638bc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="638bc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="638bc-122">id</span><span class="sxs-lookup"><span data-stu-id="638bc-122">id</span></span>|<span data-ttu-id="638bc-123">String</span><span class="sxs-lookup"><span data-stu-id="638bc-123">String</span></span>|<span data-ttu-id="638bc-124">Ключ сущности сводки работоспособности приложения управления, Windows.</span><span class="sxs-lookup"><span data-stu-id="638bc-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="638bc-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="638bc-125">healthyDeviceCount</span></span>|<span data-ttu-id="638bc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="638bc-126">Int32</span></span>|<span data-ttu-id="638bc-127">Счетчик работоспособном устройства.</span><span class="sxs-lookup"><span data-stu-id="638bc-127">Healthy device count.</span></span>|
|<span data-ttu-id="638bc-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="638bc-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="638bc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="638bc-129">Int32</span></span>|<span data-ttu-id="638bc-130">Счетчик неработоспособные устройства.</span><span class="sxs-lookup"><span data-stu-id="638bc-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="638bc-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="638bc-131">unknownDeviceCount</span></span>|<span data-ttu-id="638bc-132">Int32</span><span class="sxs-lookup"><span data-stu-id="638bc-132">Int32</span></span>|<span data-ttu-id="638bc-133">Счетчик неизвестные устройства.</span><span class="sxs-lookup"><span data-stu-id="638bc-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="638bc-134">Связи</span><span class="sxs-lookup"><span data-stu-id="638bc-134">Relationships</span></span>
<span data-ttu-id="638bc-135">Нет</span><span class="sxs-lookup"><span data-stu-id="638bc-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="638bc-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="638bc-136">JSON Representation</span></span>
<span data-ttu-id="638bc-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="638bc-137">Here is a JSON representation of the resource.</span></span>
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





