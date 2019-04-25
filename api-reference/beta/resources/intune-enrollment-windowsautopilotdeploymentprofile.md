---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Профиль развертывания Windows для автопилота
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f82d48422ecff99f106d4a62b07ac8532cb546c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546999"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="e303f-103">Тип ресурса windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="e303f-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="e303f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e303f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e303f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e303f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e303f-106">Профиль развертывания Windows для автопилота</span><span class="sxs-lookup"><span data-stu-id="e303f-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="e303f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e303f-107">Methods</span></span>
|<span data-ttu-id="e303f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e303f-108">Method</span></span>|<span data-ttu-id="e303f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e303f-109">Return Type</span></span>|<span data-ttu-id="e303f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e303f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e303f-111">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="e303f-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="e303f-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="e303f-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="e303f-113">Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e303f-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="e303f-114">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e303f-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="e303f-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e303f-115">None</span></span>|<span data-ttu-id="e303f-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e303f-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e303f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e303f-117">Properties</span></span>
|<span data-ttu-id="e303f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e303f-118">Property</span></span>|<span data-ttu-id="e303f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e303f-119">Type</span></span>|<span data-ttu-id="e303f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e303f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e303f-121">id</span><span class="sxs-lookup"><span data-stu-id="e303f-121">id</span></span>|<span data-ttu-id="e303f-122">Строка</span><span class="sxs-lookup"><span data-stu-id="e303f-122">String</span></span>|<span data-ttu-id="e303f-123">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="e303f-123">Profile Key</span></span>|
|<span data-ttu-id="e303f-124">displayName</span><span class="sxs-lookup"><span data-stu-id="e303f-124">displayName</span></span>|<span data-ttu-id="e303f-125">Строка</span><span class="sxs-lookup"><span data-stu-id="e303f-125">String</span></span>|<span data-ttu-id="e303f-126">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="e303f-126">Name of the profile</span></span>|
|<span data-ttu-id="e303f-127">description</span><span class="sxs-lookup"><span data-stu-id="e303f-127">description</span></span>|<span data-ttu-id="e303f-128">String</span><span class="sxs-lookup"><span data-stu-id="e303f-128">String</span></span>|<span data-ttu-id="e303f-129">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="e303f-129">Description of the profile</span></span>|
|<span data-ttu-id="e303f-130">language</span><span class="sxs-lookup"><span data-stu-id="e303f-130">language</span></span>|<span data-ttu-id="e303f-131">String</span><span class="sxs-lookup"><span data-stu-id="e303f-131">String</span></span>|<span data-ttu-id="e303f-132">Язык, настроенный на устройстве</span><span class="sxs-lookup"><span data-stu-id="e303f-132">Language configured on the device</span></span>|
|<span data-ttu-id="e303f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e303f-133">createdDateTime</span></span>|<span data-ttu-id="e303f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e303f-134">DateTimeOffset</span></span>|<span data-ttu-id="e303f-135">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="e303f-135">Profile creation time</span></span>|
|<span data-ttu-id="e303f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e303f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e303f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e303f-137">DateTimeOffset</span></span>|<span data-ttu-id="e303f-138">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="e303f-138">Profile last modified time</span></span>|
|<span data-ttu-id="e303f-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e303f-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="e303f-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e303f-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="e303f-141">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="e303f-141">Out of box experience setting</span></span>|
|<span data-ttu-id="e303f-142">Енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="e303f-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="e303f-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="e303f-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="e303f-144">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="e303f-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="e303f-145">Екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="e303f-145">extractHardwareHash</span></span>|<span data-ttu-id="e303f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="e303f-146">Boolean</span></span>|<span data-ttu-id="e303f-147">Извлечение Хардварехаш для профиля</span><span class="sxs-lookup"><span data-stu-id="e303f-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="e303f-148">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="e303f-148">deviceNameTemplate</span></span>|<span data-ttu-id="e303f-149">String</span><span class="sxs-lookup"><span data-stu-id="e303f-149">String</span></span>|<span data-ttu-id="e303f-150">Шаблон, используемый для именования автоПилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="e303f-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="e303f-151">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="e303f-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="e303f-152">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="e303f-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="e303f-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="e303f-153">deviceType</span></span>|[<span data-ttu-id="e303f-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="e303f-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="e303f-155">Тип устройства автоПилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="e303f-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="e303f-156">Возможные значения: `windowsPc`, `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="e303f-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="e303f-157">Енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="e303f-157">enableWhiteGlove</span></span>|<span data-ttu-id="e303f-158">Логический</span><span class="sxs-lookup"><span data-stu-id="e303f-158">Boolean</span></span>|<span data-ttu-id="e303f-159">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="e303f-159">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e303f-160">Связи</span><span class="sxs-lookup"><span data-stu-id="e303f-160">Relationships</span></span>
|<span data-ttu-id="e303f-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="e303f-161">Relationship</span></span>|<span data-ttu-id="e303f-162">Тип</span><span class="sxs-lookup"><span data-stu-id="e303f-162">Type</span></span>|<span data-ttu-id="e303f-163">Описание</span><span class="sxs-lookup"><span data-stu-id="e303f-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e303f-164">Ассигнеддевицес</span><span class="sxs-lookup"><span data-stu-id="e303f-164">assignedDevices</span></span>|<span data-ttu-id="e303f-165">Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="e303f-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="e303f-166">Список назначенных устройств для профиля.</span><span class="sxs-lookup"><span data-stu-id="e303f-166">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="e303f-167">assignments</span><span class="sxs-lookup"><span data-stu-id="e303f-167">assignments</span></span>|<span data-ttu-id="e303f-168">Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e303f-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="e303f-169">Список назначений групп для профиля.</span><span class="sxs-lookup"><span data-stu-id="e303f-169">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e303f-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e303f-170">JSON Representation</span></span>
<span data-ttu-id="e303f-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e303f-171">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true
}
```





