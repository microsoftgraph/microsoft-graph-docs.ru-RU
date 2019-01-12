---
title: Тип ресурса mobileAppTroubleshootingEvent
description: Событие, представляющее приложение устройства пользователей установить состояние.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d26873b90941f27538a5c71e113a92bb5af1bf26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977327"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="e67cf-103">Тип ресурса mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e67cf-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="e67cf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e67cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e67cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e67cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e67cf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e67cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e67cf-107">Событие, представляющее приложение устройства пользователей установить состояние.</span><span class="sxs-lookup"><span data-stu-id="e67cf-107">Event representing a users device application install status.</span></span>

<span data-ttu-id="e67cf-108">Наследуется от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e67cf-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e67cf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e67cf-109">Methods</span></span>
|<span data-ttu-id="e67cf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e67cf-110">Method</span></span>|<span data-ttu-id="e67cf-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e67cf-111">Return Type</span></span>|<span data-ttu-id="e67cf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e67cf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e67cf-113">Список mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="e67cf-113">List mobileAppTroubleshootingEvents</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="e67cf-114">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e67cf-114">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="e67cf-115">Свойства списка и связей объектов [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e67cf-115">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="e67cf-116">Получение mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e67cf-116">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|<span data-ttu-id="e67cf-117">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md);</span><span class="sxs-lookup"><span data-stu-id="e67cf-117">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)</span></span>|<span data-ttu-id="e67cf-118">Чтение свойства и связи объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e67cf-118">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="e67cf-119">Создание mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e67cf-119">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|<span data-ttu-id="e67cf-120">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md);</span><span class="sxs-lookup"><span data-stu-id="e67cf-120">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)</span></span>|<span data-ttu-id="e67cf-121">Создание нового объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e67cf-121">Create a new [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="e67cf-122">Удаление mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e67cf-122">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="e67cf-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e67cf-123">None</span></span>|<span data-ttu-id="e67cf-124">Удаляет [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e67cf-124">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="e67cf-125">Обновление mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e67cf-125">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|<span data-ttu-id="e67cf-126">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md);</span><span class="sxs-lookup"><span data-stu-id="e67cf-126">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)</span></span>|<span data-ttu-id="e67cf-127">Обновление свойства объекта [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="e67cf-127">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e67cf-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="e67cf-128">Properties</span></span>
|<span data-ttu-id="e67cf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e67cf-129">Property</span></span>|<span data-ttu-id="e67cf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e67cf-130">Type</span></span>|<span data-ttu-id="e67cf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e67cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e67cf-132">id</span><span class="sxs-lookup"><span data-stu-id="e67cf-132">id</span></span>|<span data-ttu-id="e67cf-133">String</span><span class="sxs-lookup"><span data-stu-id="e67cf-133">String</span></span>|<span data-ttu-id="e67cf-134">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e67cf-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e67cf-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e67cf-135">eventDateTime</span></span>|<span data-ttu-id="e67cf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e67cf-136">DateTimeOffset</span></span>|<span data-ttu-id="e67cf-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="e67cf-137">Time when the event occurred .</span></span> <span data-ttu-id="e67cf-138">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e67cf-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e67cf-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="e67cf-139">correlationId</span></span>|<span data-ttu-id="e67cf-140">String</span><span class="sxs-lookup"><span data-stu-id="e67cf-140">String</span></span>|<span data-ttu-id="e67cf-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="e67cf-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="e67cf-142">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e67cf-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e67cf-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e67cf-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="e67cf-144">String</span><span class="sxs-lookup"><span data-stu-id="e67cf-144">String</span></span>|<span data-ttu-id="e67cf-145">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="e67cf-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e67cf-146">userId</span><span class="sxs-lookup"><span data-stu-id="e67cf-146">userId</span></span>|<span data-ttu-id="e67cf-147">String</span><span class="sxs-lookup"><span data-stu-id="e67cf-147">String</span></span>|<span data-ttu-id="e67cf-148">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="e67cf-148">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e67cf-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="e67cf-149">applicationId</span></span>|<span data-ttu-id="e67cf-150">String</span><span class="sxs-lookup"><span data-stu-id="e67cf-150">String</span></span>|<span data-ttu-id="e67cf-151">Идентификатор приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="e67cf-151">Intune application identifier.</span></span>|
|<span data-ttu-id="e67cf-152">журнал</span><span class="sxs-lookup"><span data-stu-id="e67cf-152">history</span></span>|<span data-ttu-id="e67cf-153">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e67cf-153">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="e67cf-154">Устранение неполадок в элемент журнала Intune мобильного приложения</span><span class="sxs-lookup"><span data-stu-id="e67cf-154">Intune Mobile Application Troubleshooting History Item</span></span>|

## <a name="relationships"></a><span data-ttu-id="e67cf-155">Связи</span><span class="sxs-lookup"><span data-stu-id="e67cf-155">Relationships</span></span>
<span data-ttu-id="e67cf-156">Нет</span><span class="sxs-lookup"><span data-stu-id="e67cf-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e67cf-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e67cf-157">JSON Representation</span></span>
<span data-ttu-id="e67cf-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e67cf-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```





