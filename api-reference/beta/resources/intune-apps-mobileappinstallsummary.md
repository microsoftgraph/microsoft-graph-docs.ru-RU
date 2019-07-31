---
title: Тип ресурса Мобилеаппинсталлсуммари
description: Содержит свойства для сводки установки мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e836ba4458c72b9ab017fe499634caec79cce551
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012452"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="282d2-103">Тип ресурса Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="282d2-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="282d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="282d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="282d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="282d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="282d2-106">Содержит свойства для сводки установки мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="282d2-106">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="282d2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="282d2-107">Methods</span></span>
|<span data-ttu-id="282d2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="282d2-108">Method</span></span>|<span data-ttu-id="282d2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="282d2-109">Return Type</span></span>|<span data-ttu-id="282d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="282d2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="282d2-111">Получение Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="282d2-111">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|<span data-ttu-id="282d2-112">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="282d2-112">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="282d2-113">Чтение свойств и связей объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="282d2-113">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="282d2-114">Обновление Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="282d2-114">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|<span data-ttu-id="282d2-115">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="282d2-115">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="282d2-116">Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="282d2-116">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="282d2-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="282d2-117">Properties</span></span>
|<span data-ttu-id="282d2-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="282d2-118">Property</span></span>|<span data-ttu-id="282d2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="282d2-119">Type</span></span>|<span data-ttu-id="282d2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="282d2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="282d2-121">id</span><span class="sxs-lookup"><span data-stu-id="282d2-121">id</span></span>|<span data-ttu-id="282d2-122">String</span><span class="sxs-lookup"><span data-stu-id="282d2-122">String</span></span>|<span data-ttu-id="282d2-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="282d2-123">Key of the entity.</span></span>|
|<span data-ttu-id="282d2-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="282d2-124">installedDeviceCount</span></span>|<span data-ttu-id="282d2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-125">Int32</span></span>|<span data-ttu-id="282d2-126">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="282d2-126">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="282d2-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="282d2-127">failedDeviceCount</span></span>|<span data-ttu-id="282d2-128">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-128">Int32</span></span>|<span data-ttu-id="282d2-129">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="282d2-129">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="282d2-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="282d2-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="282d2-131">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-131">Int32</span></span>|<span data-ttu-id="282d2-132">Количество устройств, неприменимых к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="282d2-132">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="282d2-133">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="282d2-133">notInstalledDeviceCount</span></span>|<span data-ttu-id="282d2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-134">Int32</span></span>|<span data-ttu-id="282d2-135">Количество устройств, на которых не установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="282d2-135">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="282d2-136">Пендингинсталлдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="282d2-136">pendingInstallDeviceCount</span></span>|<span data-ttu-id="282d2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-137">Int32</span></span>|<span data-ttu-id="282d2-138">Количество устройств, которые были уведомлены об установке этого приложения.</span><span class="sxs-lookup"><span data-stu-id="282d2-138">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="282d2-139">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="282d2-139">installedUserCount</span></span>|<span data-ttu-id="282d2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-140">Int32</span></span>|<span data-ttu-id="282d2-141">Количество пользователей, чьи устройства успешно выполнили установку этого приложения.</span><span class="sxs-lookup"><span data-stu-id="282d2-141">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="282d2-142">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="282d2-142">failedUserCount</span></span>|<span data-ttu-id="282d2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-143">Int32</span></span>|<span data-ttu-id="282d2-144">Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="282d2-144">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="282d2-145">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="282d2-145">notApplicableUserCount</span></span>|<span data-ttu-id="282d2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-146">Int32</span></span>|<span data-ttu-id="282d2-147">Количество пользователей, чьи устройства были неприменимы к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="282d2-147">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="282d2-148">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="282d2-148">notInstalledUserCount</span></span>|<span data-ttu-id="282d2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-149">Int32</span></span>|<span data-ttu-id="282d2-150">Количество пользователей с 1 или больше устройств, которые не установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="282d2-150">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="282d2-151">Пендингинсталлусеркаунт</span><span class="sxs-lookup"><span data-stu-id="282d2-151">pendingInstallUserCount</span></span>|<span data-ttu-id="282d2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="282d2-152">Int32</span></span>|<span data-ttu-id="282d2-153">Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="282d2-153">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="282d2-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="282d2-154">Relationships</span></span>
<span data-ttu-id="282d2-155">Нет</span><span class="sxs-lookup"><span data-stu-id="282d2-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="282d2-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="282d2-156">JSON Representation</span></span>
<span data-ttu-id="282d2-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="282d2-157">Here is a JSON representation of the resource.</span></span>
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





