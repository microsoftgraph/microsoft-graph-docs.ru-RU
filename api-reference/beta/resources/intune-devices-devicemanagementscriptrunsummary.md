---
title: Тип ресурса deviceManagementScriptRunSummary
description: Содержит свойства для выполнения Сводка сценарий управления устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9676fc7f6792c3bd9771ab7ed1ccbeaa67826d3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962039"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="010ae-103">Тип ресурса deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="010ae-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="010ae-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="010ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="010ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="010ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="010ae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="010ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="010ae-107">Содержит свойства для выполнения Сводка сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="010ae-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="010ae-108">Методы</span><span class="sxs-lookup"><span data-stu-id="010ae-108">Methods</span></span>
|<span data-ttu-id="010ae-109">Метод</span><span class="sxs-lookup"><span data-stu-id="010ae-109">Method</span></span>|<span data-ttu-id="010ae-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="010ae-110">Return Type</span></span>|<span data-ttu-id="010ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="010ae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="010ae-112">Получение deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="010ae-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|<span data-ttu-id="010ae-113">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);</span><span class="sxs-lookup"><span data-stu-id="010ae-113">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span></span>|<span data-ttu-id="010ae-114">Чтение свойства и связи объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="010ae-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="010ae-115">Обновление deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="010ae-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|<span data-ttu-id="010ae-116">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);</span><span class="sxs-lookup"><span data-stu-id="010ae-116">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span></span>|<span data-ttu-id="010ae-117">Обновление свойства объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="010ae-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="010ae-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="010ae-118">Properties</span></span>
|<span data-ttu-id="010ae-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="010ae-119">Property</span></span>|<span data-ttu-id="010ae-120">Тип</span><span class="sxs-lookup"><span data-stu-id="010ae-120">Type</span></span>|<span data-ttu-id="010ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="010ae-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="010ae-122">id</span><span class="sxs-lookup"><span data-stu-id="010ae-122">id</span></span>|<span data-ttu-id="010ae-123">String</span><span class="sxs-lookup"><span data-stu-id="010ae-123">String</span></span>|<span data-ttu-id="010ae-124">Клавиша сценарий управления устройства выполните сводки сущности.</span><span class="sxs-lookup"><span data-stu-id="010ae-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="010ae-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="010ae-125">successDeviceCount</span></span>|<span data-ttu-id="010ae-126">Int32</span><span class="sxs-lookup"><span data-stu-id="010ae-126">Int32</span></span>|<span data-ttu-id="010ae-127">Число допустимых устройства.</span><span class="sxs-lookup"><span data-stu-id="010ae-127">Success device count.</span></span>|
|<span data-ttu-id="010ae-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="010ae-128">errorDeviceCount</span></span>|<span data-ttu-id="010ae-129">Int32</span><span class="sxs-lookup"><span data-stu-id="010ae-129">Int32</span></span>|<span data-ttu-id="010ae-130">Число ошибок устройства.</span><span class="sxs-lookup"><span data-stu-id="010ae-130">Error device count.</span></span>|
|<span data-ttu-id="010ae-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="010ae-131">successUserCount</span></span>|<span data-ttu-id="010ae-132">Int32</span><span class="sxs-lookup"><span data-stu-id="010ae-132">Int32</span></span>|<span data-ttu-id="010ae-133">Число пользователей успеха.</span><span class="sxs-lookup"><span data-stu-id="010ae-133">Success user count.</span></span>|
|<span data-ttu-id="010ae-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="010ae-134">errorUserCount</span></span>|<span data-ttu-id="010ae-135">Int32</span><span class="sxs-lookup"><span data-stu-id="010ae-135">Int32</span></span>|<span data-ttu-id="010ae-136">Число пользователей об ошибках.</span><span class="sxs-lookup"><span data-stu-id="010ae-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="010ae-137">Связи</span><span class="sxs-lookup"><span data-stu-id="010ae-137">Relationships</span></span>
<span data-ttu-id="010ae-138">Нет</span><span class="sxs-lookup"><span data-stu-id="010ae-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="010ae-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="010ae-139">JSON Representation</span></span>
<span data-ttu-id="010ae-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="010ae-140">Here is a JSON representation of the resource.</span></span>
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





