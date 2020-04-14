---
title: Тип ресурса Мобилеаппинсталлсуммари
description: Содержит свойства для сводки установки мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d6ee038510ce7891e2599dda2d101ed7d1aec6d1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457011"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="90746-103">Тип ресурса Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="90746-103">mobileAppInstallSummary resource type</span></span>

<span data-ttu-id="90746-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90746-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90746-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90746-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90746-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90746-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90746-107">Содержит свойства для сводки установки мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="90746-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="90746-108">Методы</span><span class="sxs-lookup"><span data-stu-id="90746-108">Methods</span></span>
|<span data-ttu-id="90746-109">Метод</span><span class="sxs-lookup"><span data-stu-id="90746-109">Method</span></span>|<span data-ttu-id="90746-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90746-110">Return Type</span></span>|<span data-ttu-id="90746-111">Описание</span><span class="sxs-lookup"><span data-stu-id="90746-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90746-112">Получение Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="90746-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|<span data-ttu-id="90746-113">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="90746-113">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="90746-114">Чтение свойств и связей объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="90746-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="90746-115">Обновление Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="90746-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|<span data-ttu-id="90746-116">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="90746-116">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="90746-117">Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="90746-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90746-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="90746-118">Properties</span></span>
|<span data-ttu-id="90746-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="90746-119">Property</span></span>|<span data-ttu-id="90746-120">Тип</span><span class="sxs-lookup"><span data-stu-id="90746-120">Type</span></span>|<span data-ttu-id="90746-121">Описание</span><span class="sxs-lookup"><span data-stu-id="90746-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90746-122">id</span><span class="sxs-lookup"><span data-stu-id="90746-122">id</span></span>|<span data-ttu-id="90746-123">String</span><span class="sxs-lookup"><span data-stu-id="90746-123">String</span></span>|<span data-ttu-id="90746-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90746-124">Key of the entity.</span></span>|
|<span data-ttu-id="90746-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90746-125">installedDeviceCount</span></span>|<span data-ttu-id="90746-126">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-126">Int32</span></span>|<span data-ttu-id="90746-127">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="90746-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="90746-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90746-128">failedDeviceCount</span></span>|<span data-ttu-id="90746-129">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-129">Int32</span></span>|<span data-ttu-id="90746-130">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="90746-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="90746-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90746-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="90746-132">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-132">Int32</span></span>|<span data-ttu-id="90746-133">Количество устройств, неприменимых к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="90746-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="90746-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90746-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="90746-135">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-135">Int32</span></span>|<span data-ttu-id="90746-136">Количество устройств, на которых не установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="90746-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="90746-137">пендингинсталлдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="90746-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="90746-138">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-138">Int32</span></span>|<span data-ttu-id="90746-139">Количество устройств, которые были уведомлены об установке этого приложения.</span><span class="sxs-lookup"><span data-stu-id="90746-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="90746-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="90746-140">installedUserCount</span></span>|<span data-ttu-id="90746-141">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-141">Int32</span></span>|<span data-ttu-id="90746-142">Количество пользователей, чьи устройства успешно выполнили установку этого приложения.</span><span class="sxs-lookup"><span data-stu-id="90746-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="90746-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="90746-143">failedUserCount</span></span>|<span data-ttu-id="90746-144">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-144">Int32</span></span>|<span data-ttu-id="90746-145">Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="90746-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="90746-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="90746-146">notApplicableUserCount</span></span>|<span data-ttu-id="90746-147">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-147">Int32</span></span>|<span data-ttu-id="90746-148">Количество пользователей, чьи устройства были неприменимы к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="90746-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="90746-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="90746-149">notInstalledUserCount</span></span>|<span data-ttu-id="90746-150">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-150">Int32</span></span>|<span data-ttu-id="90746-151">Количество пользователей с 1 или больше устройств, которые не установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="90746-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="90746-152">пендингинсталлусеркаунт</span><span class="sxs-lookup"><span data-stu-id="90746-152">pendingInstallUserCount</span></span>|<span data-ttu-id="90746-153">Int32</span><span class="sxs-lookup"><span data-stu-id="90746-153">Int32</span></span>|<span data-ttu-id="90746-154">Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="90746-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90746-155">Связи</span><span class="sxs-lookup"><span data-stu-id="90746-155">Relationships</span></span>
<span data-ttu-id="90746-156">Нет</span><span class="sxs-lookup"><span data-stu-id="90746-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90746-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90746-157">JSON Representation</span></span>
<span data-ttu-id="90746-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90746-158">Here is a JSON representation of the resource.</span></span>
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



