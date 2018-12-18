---
title: Тип ресурса deviceManagementScriptRunSummary
description: Содержит свойства для выполнения Сводка сценарий управления устройства.
author: tfitzmac
ms.openlocfilehash: 347a4e5cd3c4201949841054b69c217ad4f9fa8e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338999"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="cffe1-103">Тип ресурса deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cffe1-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="cffe1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cffe1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cffe1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cffe1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cffe1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cffe1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cffe1-107">Содержит свойства для выполнения Сводка сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="cffe1-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="cffe1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cffe1-108">Methods</span></span>
|<span data-ttu-id="cffe1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cffe1-109">Method</span></span>|<span data-ttu-id="cffe1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cffe1-110">Return Type</span></span>|<span data-ttu-id="cffe1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cffe1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cffe1-112">Получение deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cffe1-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|<span data-ttu-id="cffe1-113">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);</span><span class="sxs-lookup"><span data-stu-id="cffe1-113">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span></span>|<span data-ttu-id="cffe1-114">Чтение свойства и связи объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cffe1-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="cffe1-115">Обновление deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cffe1-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|<span data-ttu-id="cffe1-116">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);</span><span class="sxs-lookup"><span data-stu-id="cffe1-116">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span></span>|<span data-ttu-id="cffe1-117">Обновление свойства объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cffe1-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cffe1-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cffe1-118">Properties</span></span>
|<span data-ttu-id="cffe1-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cffe1-119">Property</span></span>|<span data-ttu-id="cffe1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cffe1-120">Type</span></span>|<span data-ttu-id="cffe1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cffe1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cffe1-122">id</span><span class="sxs-lookup"><span data-stu-id="cffe1-122">id</span></span>|<span data-ttu-id="cffe1-123">Строка</span><span class="sxs-lookup"><span data-stu-id="cffe1-123">String</span></span>|<span data-ttu-id="cffe1-124">Клавиша сценарий управления устройства выполните сводки сущности.</span><span class="sxs-lookup"><span data-stu-id="cffe1-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="cffe1-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cffe1-125">successDeviceCount</span></span>|<span data-ttu-id="cffe1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cffe1-126">Int32</span></span>|<span data-ttu-id="cffe1-127">Число допустимых устройства.</span><span class="sxs-lookup"><span data-stu-id="cffe1-127">Success device count.</span></span>|
|<span data-ttu-id="cffe1-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cffe1-128">errorDeviceCount</span></span>|<span data-ttu-id="cffe1-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cffe1-129">Int32</span></span>|<span data-ttu-id="cffe1-130">Число ошибок устройства.</span><span class="sxs-lookup"><span data-stu-id="cffe1-130">Error device count.</span></span>|
|<span data-ttu-id="cffe1-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="cffe1-131">successUserCount</span></span>|<span data-ttu-id="cffe1-132">Int32</span><span class="sxs-lookup"><span data-stu-id="cffe1-132">Int32</span></span>|<span data-ttu-id="cffe1-133">Число пользователей успеха.</span><span class="sxs-lookup"><span data-stu-id="cffe1-133">Success user count.</span></span>|
|<span data-ttu-id="cffe1-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="cffe1-134">errorUserCount</span></span>|<span data-ttu-id="cffe1-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cffe1-135">Int32</span></span>|<span data-ttu-id="cffe1-136">Число пользователей об ошибках.</span><span class="sxs-lookup"><span data-stu-id="cffe1-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cffe1-137">Связи</span><span class="sxs-lookup"><span data-stu-id="cffe1-137">Relationships</span></span>
<span data-ttu-id="cffe1-138">Нет</span><span class="sxs-lookup"><span data-stu-id="cffe1-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cffe1-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cffe1-139">JSON Representation</span></span>
<span data-ttu-id="cffe1-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cffe1-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```





