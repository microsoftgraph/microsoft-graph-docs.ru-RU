---
title: Тип ресурса mobileAppInstallSummary
description: Содержит свойства для установки сведениям о мобильных приложений.
ms.openlocfilehash: bda3f798a86b38ca0d1224ce509c355a8aec998a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075290"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="0cf81-103">Тип ресурса mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0cf81-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="0cf81-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0cf81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cf81-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cf81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cf81-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0cf81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cf81-107">Содержит свойства для установки сведениям о мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="0cf81-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="0cf81-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0cf81-108">Methods</span></span>
|<span data-ttu-id="0cf81-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0cf81-109">Method</span></span>|<span data-ttu-id="0cf81-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0cf81-110">Return Type</span></span>|<span data-ttu-id="0cf81-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0cf81-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0cf81-112">Получение mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0cf81-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|<span data-ttu-id="0cf81-113">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="0cf81-113">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="0cf81-114">Чтение свойства и связи объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0cf81-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="0cf81-115">Обновление mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0cf81-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|<span data-ttu-id="0cf81-116">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="0cf81-116">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="0cf81-117">Обновление свойства объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0cf81-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cf81-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cf81-118">Properties</span></span>
|<span data-ttu-id="0cf81-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cf81-119">Property</span></span>|<span data-ttu-id="0cf81-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0cf81-120">Type</span></span>|<span data-ttu-id="0cf81-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0cf81-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf81-122">id</span><span class="sxs-lookup"><span data-stu-id="0cf81-122">id</span></span>|<span data-ttu-id="0cf81-123">String</span><span class="sxs-lookup"><span data-stu-id="0cf81-123">String</span></span>|<span data-ttu-id="0cf81-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0cf81-124">Key of the entity.</span></span>|
|<span data-ttu-id="0cf81-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-125">installedDeviceCount</span></span>|<span data-ttu-id="0cf81-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-126">Int32</span></span>|<span data-ttu-id="0cf81-127">Количество устройств, которые были успешно установлены этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0cf81-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="0cf81-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-128">failedDeviceCount</span></span>|<span data-ttu-id="0cf81-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-129">Int32</span></span>|<span data-ttu-id="0cf81-130">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="0cf81-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="0cf81-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="0cf81-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-132">Int32</span></span>|<span data-ttu-id="0cf81-133">Количество устройств, которые не применимы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0cf81-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="0cf81-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="0cf81-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-135">Int32</span></span>|<span data-ttu-id="0cf81-136">Количество устройств, для которого не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="0cf81-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="0cf81-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="0cf81-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-138">Int32</span></span>|<span data-ttu-id="0cf81-139">Количество устройств, которые были уведомлены для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0cf81-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="0cf81-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-140">installedUserCount</span></span>|<span data-ttu-id="0cf81-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-141">Int32</span></span>|<span data-ttu-id="0cf81-142">Число пользователей, чьи устройств успешно для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0cf81-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="0cf81-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-143">failedUserCount</span></span>|<span data-ttu-id="0cf81-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-144">Int32</span></span>|<span data-ttu-id="0cf81-145">Число пользователей, имеющих 1 или другие устройства, который не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="0cf81-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="0cf81-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-146">notApplicableUserCount</span></span>|<span data-ttu-id="0cf81-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-147">Int32</span></span>|<span data-ttu-id="0cf81-148">Число пользователей, которых устройства не все для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0cf81-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="0cf81-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-149">notInstalledUserCount</span></span>|<span data-ttu-id="0cf81-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-150">Int32</span></span>|<span data-ttu-id="0cf81-151">Число пользователей, которые имеют 1 или более устройства, на которых не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="0cf81-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="0cf81-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="0cf81-152">pendingInstallUserCount</span></span>|<span data-ttu-id="0cf81-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf81-153">Int32</span></span>|<span data-ttu-id="0cf81-154">Число пользователей, имеющих 1 или другие устройства, уведомлены для установки этого приложения и 0 устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="0cf81-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cf81-155">Связи</span><span class="sxs-lookup"><span data-stu-id="0cf81-155">Relationships</span></span>
<span data-ttu-id="0cf81-156">Нет</span><span class="sxs-lookup"><span data-stu-id="0cf81-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0cf81-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cf81-157">JSON Representation</span></span>
<span data-ttu-id="0cf81-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cf81-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```





