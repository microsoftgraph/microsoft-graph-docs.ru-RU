---
title: Тип ресурса windowsManagementAppHealthSummary
description: Содержит свойства для Сводка работоспособности приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d2e8dbc0af1d814ecd47210c4def5a7c7e02edd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967461"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="b1b79-103">Тип ресурса windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="b1b79-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="b1b79-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b1b79-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1b79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1b79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1b79-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b1b79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1b79-107">Содержит свойства для Сводка работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="b1b79-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="b1b79-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b1b79-108">Methods</span></span>
|<span data-ttu-id="b1b79-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b1b79-109">Method</span></span>|<span data-ttu-id="b1b79-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1b79-110">Return Type</span></span>|<span data-ttu-id="b1b79-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b79-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1b79-112">Получение windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="b1b79-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|<span data-ttu-id="b1b79-113">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b1b79-113">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="b1b79-114">Чтение свойства и связи объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b1b79-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="b1b79-115">Обновление windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="b1b79-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|<span data-ttu-id="b1b79-116">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b1b79-116">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="b1b79-117">Обновление свойства объекта [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b1b79-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1b79-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1b79-118">Properties</span></span>
|<span data-ttu-id="b1b79-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1b79-119">Property</span></span>|<span data-ttu-id="b1b79-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b1b79-120">Type</span></span>|<span data-ttu-id="b1b79-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b79-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b79-122">id</span><span class="sxs-lookup"><span data-stu-id="b1b79-122">id</span></span>|<span data-ttu-id="b1b79-123">Строка</span><span class="sxs-lookup"><span data-stu-id="b1b79-123">String</span></span>|<span data-ttu-id="b1b79-124">Ключ сущности сводки работоспособности приложения управления, Windows.</span><span class="sxs-lookup"><span data-stu-id="b1b79-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="b1b79-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1b79-125">healthyDeviceCount</span></span>|<span data-ttu-id="b1b79-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b79-126">Int32</span></span>|<span data-ttu-id="b1b79-127">Счетчик работоспособном устройства.</span><span class="sxs-lookup"><span data-stu-id="b1b79-127">Healthy device count.</span></span>|
|<span data-ttu-id="b1b79-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1b79-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="b1b79-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b79-129">Int32</span></span>|<span data-ttu-id="b1b79-130">Счетчик неработоспособные устройства.</span><span class="sxs-lookup"><span data-stu-id="b1b79-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="b1b79-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1b79-131">unknownDeviceCount</span></span>|<span data-ttu-id="b1b79-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b79-132">Int32</span></span>|<span data-ttu-id="b1b79-133">Счетчик неизвестные устройства.</span><span class="sxs-lookup"><span data-stu-id="b1b79-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1b79-134">Связи</span><span class="sxs-lookup"><span data-stu-id="b1b79-134">Relationships</span></span>
<span data-ttu-id="b1b79-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b1b79-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1b79-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1b79-136">JSON Representation</span></span>
<span data-ttu-id="b1b79-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1b79-137">Here is a JSON representation of the resource.</span></span>
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





