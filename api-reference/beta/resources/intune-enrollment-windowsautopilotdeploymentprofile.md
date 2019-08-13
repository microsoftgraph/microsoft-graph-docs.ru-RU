---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Профиль развертывания Windows для автопилота
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55703bc3b531a3671b70882a18f41522dd9a5c73
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327768"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="6c258-103">Тип ресурса windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="6c258-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="6c258-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c258-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c258-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c258-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c258-106">Профиль развертывания Windows для автопилота</span><span class="sxs-lookup"><span data-stu-id="6c258-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="6c258-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6c258-107">Methods</span></span>
|<span data-ttu-id="6c258-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6c258-108">Method</span></span>|<span data-ttu-id="6c258-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c258-109">Return Type</span></span>|<span data-ttu-id="6c258-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6c258-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c258-111">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="6c258-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="6c258-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="6c258-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="6c258-113">Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6c258-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="6c258-114">Действие assign</span><span class="sxs-lookup"><span data-stu-id="6c258-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="6c258-115">Нет</span><span class="sxs-lookup"><span data-stu-id="6c258-115">None</span></span>|<span data-ttu-id="6c258-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6c258-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6c258-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c258-117">Properties</span></span>
|<span data-ttu-id="6c258-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c258-118">Property</span></span>|<span data-ttu-id="6c258-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6c258-119">Type</span></span>|<span data-ttu-id="6c258-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c258-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c258-121">id</span><span class="sxs-lookup"><span data-stu-id="6c258-121">id</span></span>|<span data-ttu-id="6c258-122">Строка</span><span class="sxs-lookup"><span data-stu-id="6c258-122">String</span></span>|<span data-ttu-id="6c258-123">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="6c258-123">Profile Key</span></span>|
|<span data-ttu-id="6c258-124">displayName</span><span class="sxs-lookup"><span data-stu-id="6c258-124">displayName</span></span>|<span data-ttu-id="6c258-125">Строка</span><span class="sxs-lookup"><span data-stu-id="6c258-125">String</span></span>|<span data-ttu-id="6c258-126">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="6c258-126">Name of the profile</span></span>|
|<span data-ttu-id="6c258-127">description</span><span class="sxs-lookup"><span data-stu-id="6c258-127">description</span></span>|<span data-ttu-id="6c258-128">String</span><span class="sxs-lookup"><span data-stu-id="6c258-128">String</span></span>|<span data-ttu-id="6c258-129">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="6c258-129">Description of the profile</span></span>|
|<span data-ttu-id="6c258-130">language</span><span class="sxs-lookup"><span data-stu-id="6c258-130">language</span></span>|<span data-ttu-id="6c258-131">String</span><span class="sxs-lookup"><span data-stu-id="6c258-131">String</span></span>|<span data-ttu-id="6c258-132">Язык, настроенный на устройстве</span><span class="sxs-lookup"><span data-stu-id="6c258-132">Language configured on the device</span></span>|
|<span data-ttu-id="6c258-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c258-133">createdDateTime</span></span>|<span data-ttu-id="6c258-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c258-134">DateTimeOffset</span></span>|<span data-ttu-id="6c258-135">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="6c258-135">Profile creation time</span></span>|
|<span data-ttu-id="6c258-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c258-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6c258-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c258-137">DateTimeOffset</span></span>|<span data-ttu-id="6c258-138">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="6c258-138">Profile last modified time</span></span>|
|<span data-ttu-id="6c258-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="6c258-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="6c258-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="6c258-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="6c258-141">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="6c258-141">Out of box experience setting</span></span>|
|<span data-ttu-id="6c258-142">енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="6c258-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="6c258-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="6c258-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="6c258-144">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="6c258-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="6c258-145">екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="6c258-145">extractHardwareHash</span></span>|<span data-ttu-id="6c258-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c258-146">Boolean</span></span>|<span data-ttu-id="6c258-147">Извлечение Хардварехаш для профиля</span><span class="sxs-lookup"><span data-stu-id="6c258-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="6c258-148">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="6c258-148">deviceNameTemplate</span></span>|<span data-ttu-id="6c258-149">String</span><span class="sxs-lookup"><span data-stu-id="6c258-149">String</span></span>|<span data-ttu-id="6c258-150">Шаблон, используемый для именования автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="6c258-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="6c258-151">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="6c258-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="6c258-152">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="6c258-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="6c258-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="6c258-153">deviceType</span></span>|[<span data-ttu-id="6c258-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="6c258-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="6c258-155">Тип устройства автопилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="6c258-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="6c258-156">Возможные значения: `windowsPc`, `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="6c258-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="6c258-157">енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="6c258-157">enableWhiteGlove</span></span>|<span data-ttu-id="6c258-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c258-158">Boolean</span></span>|<span data-ttu-id="6c258-159">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="6c258-159">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="6c258-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c258-160">roleScopeTagIds</span></span>|<span data-ttu-id="6c258-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6c258-161">String collection</span></span>|<span data-ttu-id="6c258-162">Теги областей для профиля.</span><span class="sxs-lookup"><span data-stu-id="6c258-162">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c258-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="6c258-163">Relationships</span></span>
|<span data-ttu-id="6c258-164">Отношение</span><span class="sxs-lookup"><span data-stu-id="6c258-164">Relationship</span></span>|<span data-ttu-id="6c258-165">Тип</span><span class="sxs-lookup"><span data-stu-id="6c258-165">Type</span></span>|<span data-ttu-id="6c258-166">Описание</span><span class="sxs-lookup"><span data-stu-id="6c258-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c258-167">ассигнеддевицес</span><span class="sxs-lookup"><span data-stu-id="6c258-167">assignedDevices</span></span>|<span data-ttu-id="6c258-168">Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="6c258-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="6c258-169">Список назначенных устройств для профиля.</span><span class="sxs-lookup"><span data-stu-id="6c258-169">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="6c258-170">assignments</span><span class="sxs-lookup"><span data-stu-id="6c258-170">assignments</span></span>|<span data-ttu-id="6c258-171">Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6c258-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="6c258-172">Список назначений групп для профиля.</span><span class="sxs-lookup"><span data-stu-id="6c258-172">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c258-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c258-173">JSON Representation</span></span>
<span data-ttu-id="6c258-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c258-174">Here is a JSON representation of the resource.</span></span>
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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



