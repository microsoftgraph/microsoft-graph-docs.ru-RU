---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Windows автопилот развертывания профилей
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f97603980f4e76c4dd2f63287822a1e8e984ded
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394112"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="3cb45-103">Тип ресурса windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="3cb45-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="3cb45-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3cb45-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3cb45-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cb45-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3cb45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cb45-107">Windows автопилот развертывания профилей</span><span class="sxs-lookup"><span data-stu-id="3cb45-107">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="3cb45-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3cb45-108">Methods</span></span>
|<span data-ttu-id="3cb45-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3cb45-109">Method</span></span>|<span data-ttu-id="3cb45-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3cb45-110">Return Type</span></span>|<span data-ttu-id="3cb45-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb45-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3cb45-112">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="3cb45-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="3cb45-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="3cb45-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="3cb45-114">Чтение свойства и связи объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3cb45-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="3cb45-115">Действие assign</span><span class="sxs-lookup"><span data-stu-id="3cb45-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="3cb45-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3cb45-116">None</span></span>|<span data-ttu-id="3cb45-117">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3cb45-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3cb45-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cb45-118">Properties</span></span>
|<span data-ttu-id="3cb45-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cb45-119">Property</span></span>|<span data-ttu-id="3cb45-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb45-120">Type</span></span>|<span data-ttu-id="3cb45-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb45-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb45-122">id</span><span class="sxs-lookup"><span data-stu-id="3cb45-122">id</span></span>|<span data-ttu-id="3cb45-123">String</span><span class="sxs-lookup"><span data-stu-id="3cb45-123">String</span></span>|<span data-ttu-id="3cb45-124">Клавиша профилей</span><span class="sxs-lookup"><span data-stu-id="3cb45-124">Profile Key</span></span>|
|<span data-ttu-id="3cb45-125">displayName</span><span class="sxs-lookup"><span data-stu-id="3cb45-125">displayName</span></span>|<span data-ttu-id="3cb45-126">String</span><span class="sxs-lookup"><span data-stu-id="3cb45-126">String</span></span>|<span data-ttu-id="3cb45-127">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="3cb45-127">Name of the profile</span></span>|
|<span data-ttu-id="3cb45-128">description</span><span class="sxs-lookup"><span data-stu-id="3cb45-128">description</span></span>|<span data-ttu-id="3cb45-129">String</span><span class="sxs-lookup"><span data-stu-id="3cb45-129">String</span></span>|<span data-ttu-id="3cb45-130">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="3cb45-130">Description of the profile</span></span>|
|<span data-ttu-id="3cb45-131">language</span><span class="sxs-lookup"><span data-stu-id="3cb45-131">language</span></span>|<span data-ttu-id="3cb45-132">String</span><span class="sxs-lookup"><span data-stu-id="3cb45-132">String</span></span>|<span data-ttu-id="3cb45-133">Язык, настроенных на устройстве</span><span class="sxs-lookup"><span data-stu-id="3cb45-133">Language configured on the device</span></span>|
|<span data-ttu-id="3cb45-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cb45-134">createdDateTime</span></span>|<span data-ttu-id="3cb45-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb45-135">DateTimeOffset</span></span>|<span data-ttu-id="3cb45-136">Время создания профилей</span><span class="sxs-lookup"><span data-stu-id="3cb45-136">Profile creation time</span></span>|
|<span data-ttu-id="3cb45-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cb45-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3cb45-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb45-138">DateTimeOffset</span></span>|<span data-ttu-id="3cb45-139">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="3cb45-139">Profile last modified time</span></span>|
|<span data-ttu-id="3cb45-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3cb45-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="3cb45-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="3cb45-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="3cb45-142">В соответствующем взаимодействия параметр</span><span class="sxs-lookup"><span data-stu-id="3cb45-142">Out of box experience setting</span></span>|
|<span data-ttu-id="3cb45-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="3cb45-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="3cb45-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="3cb45-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="3cb45-145">Параметр экрана состояния подачи заявок</span><span class="sxs-lookup"><span data-stu-id="3cb45-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="3cb45-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="3cb45-146">extractHardwareHash</span></span>|<span data-ttu-id="3cb45-147">Логический</span><span class="sxs-lookup"><span data-stu-id="3cb45-147">Boolean</span></span>|<span data-ttu-id="3cb45-148">Извлечение HardwareHash для профиля</span><span class="sxs-lookup"><span data-stu-id="3cb45-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="3cb45-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="3cb45-149">deviceNameTemplate</span></span>|<span data-ttu-id="3cb45-150">String</span><span class="sxs-lookup"><span data-stu-id="3cb45-150">String</span></span>|<span data-ttu-id="3cb45-151">Шаблон, используемый для имя устройства автопилот.</span><span class="sxs-lookup"><span data-stu-id="3cb45-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="3cb45-152">Это может быть настраиваемого текста, а также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="3cb45-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="3cb45-153">Общая длина текста, созданной с помощью шаблона может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="3cb45-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cb45-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="3cb45-154">Relationships</span></span>
|<span data-ttu-id="3cb45-155">Связь</span><span class="sxs-lookup"><span data-stu-id="3cb45-155">Relationship</span></span>|<span data-ttu-id="3cb45-156">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb45-156">Type</span></span>|<span data-ttu-id="3cb45-157">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb45-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb45-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="3cb45-158">assignedDevices</span></span>|<span data-ttu-id="3cb45-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3cb45-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="3cb45-160">Список устройств, назначенных для профиля.</span><span class="sxs-lookup"><span data-stu-id="3cb45-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="3cb45-161">assignments</span><span class="sxs-lookup"><span data-stu-id="3cb45-161">assignments</span></span>|<span data-ttu-id="3cb45-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3cb45-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="3cb45-163">Список назначений группы для профиля.</span><span class="sxs-lookup"><span data-stu-id="3cb45-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cb45-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3cb45-164">JSON Representation</span></span>
<span data-ttu-id="3cb45-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb45-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String"
}
```




