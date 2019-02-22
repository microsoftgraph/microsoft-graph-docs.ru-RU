---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Профиль развертывания Windows для автопилота
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3b815e0184ab9969af348338c07c3fabf0b0597
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168875"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="be052-103">Тип ресурса windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="be052-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="be052-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be052-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be052-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be052-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be052-106">Профиль развертывания Windows для автопилота</span><span class="sxs-lookup"><span data-stu-id="be052-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="be052-107">Методы</span><span class="sxs-lookup"><span data-stu-id="be052-107">Methods</span></span>
|<span data-ttu-id="be052-108">Метод</span><span class="sxs-lookup"><span data-stu-id="be052-108">Method</span></span>|<span data-ttu-id="be052-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be052-109">Return Type</span></span>|<span data-ttu-id="be052-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be052-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be052-111">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="be052-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="be052-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="be052-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="be052-113">Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="be052-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="be052-114">Действие assign</span><span class="sxs-lookup"><span data-stu-id="be052-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="be052-115">Нет</span><span class="sxs-lookup"><span data-stu-id="be052-115">None</span></span>|<span data-ttu-id="be052-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be052-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be052-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="be052-117">Properties</span></span>
|<span data-ttu-id="be052-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="be052-118">Property</span></span>|<span data-ttu-id="be052-119">Тип</span><span class="sxs-lookup"><span data-stu-id="be052-119">Type</span></span>|<span data-ttu-id="be052-120">Описание</span><span class="sxs-lookup"><span data-stu-id="be052-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be052-121">id</span><span class="sxs-lookup"><span data-stu-id="be052-121">id</span></span>|<span data-ttu-id="be052-122">String</span><span class="sxs-lookup"><span data-stu-id="be052-122">String</span></span>|<span data-ttu-id="be052-123">Ключ профиля</span><span class="sxs-lookup"><span data-stu-id="be052-123">Profile Key</span></span>|
|<span data-ttu-id="be052-124">displayName</span><span class="sxs-lookup"><span data-stu-id="be052-124">displayName</span></span>|<span data-ttu-id="be052-125">String</span><span class="sxs-lookup"><span data-stu-id="be052-125">String</span></span>|<span data-ttu-id="be052-126">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="be052-126">Name of the profile</span></span>|
|<span data-ttu-id="be052-127">description</span><span class="sxs-lookup"><span data-stu-id="be052-127">description</span></span>|<span data-ttu-id="be052-128">Строка</span><span class="sxs-lookup"><span data-stu-id="be052-128">String</span></span>|<span data-ttu-id="be052-129">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="be052-129">Description of the profile</span></span>|
|<span data-ttu-id="be052-130">language</span><span class="sxs-lookup"><span data-stu-id="be052-130">language</span></span>|<span data-ttu-id="be052-131">String</span><span class="sxs-lookup"><span data-stu-id="be052-131">String</span></span>|<span data-ttu-id="be052-132">Язык, настроенный на устройстве</span><span class="sxs-lookup"><span data-stu-id="be052-132">Language configured on the device</span></span>|
|<span data-ttu-id="be052-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be052-133">createdDateTime</span></span>|<span data-ttu-id="be052-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be052-134">DateTimeOffset</span></span>|<span data-ttu-id="be052-135">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="be052-135">Profile creation time</span></span>|
|<span data-ttu-id="be052-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be052-136">lastModifiedDateTime</span></span>|<span data-ttu-id="be052-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be052-137">DateTimeOffset</span></span>|<span data-ttu-id="be052-138">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="be052-138">Profile last modified time</span></span>|
|<span data-ttu-id="be052-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="be052-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="be052-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="be052-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="be052-141">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="be052-141">Out of box experience setting</span></span>|
|<span data-ttu-id="be052-142">Енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="be052-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="be052-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="be052-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="be052-144">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="be052-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="be052-145">Екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="be052-145">extractHardwareHash</span></span>|<span data-ttu-id="be052-146">Логический</span><span class="sxs-lookup"><span data-stu-id="be052-146">Boolean</span></span>|<span data-ttu-id="be052-147">Извлечение Хардварехаш для профиля</span><span class="sxs-lookup"><span data-stu-id="be052-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="be052-148">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="be052-148">deviceNameTemplate</span></span>|<span data-ttu-id="be052-149">String</span><span class="sxs-lookup"><span data-stu-id="be052-149">String</span></span>|<span data-ttu-id="be052-150">Шаблон, используемый для именования автоПилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="be052-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="be052-151">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="be052-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="be052-152">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="be052-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="be052-153">Енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="be052-153">enableWhiteGlove</span></span>|<span data-ttu-id="be052-154">Логический</span><span class="sxs-lookup"><span data-stu-id="be052-154">Boolean</span></span>|<span data-ttu-id="be052-155">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="be052-155">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be052-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="be052-156">Relationships</span></span>
|<span data-ttu-id="be052-157">Связь</span><span class="sxs-lookup"><span data-stu-id="be052-157">Relationship</span></span>|<span data-ttu-id="be052-158">Тип</span><span class="sxs-lookup"><span data-stu-id="be052-158">Type</span></span>|<span data-ttu-id="be052-159">Описание</span><span class="sxs-lookup"><span data-stu-id="be052-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be052-160">Ассигнеддевицес</span><span class="sxs-lookup"><span data-stu-id="be052-160">assignedDevices</span></span>|<span data-ttu-id="be052-161">Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="be052-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="be052-162">Список назначенных устройств для профиля.</span><span class="sxs-lookup"><span data-stu-id="be052-162">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="be052-163">assignments</span><span class="sxs-lookup"><span data-stu-id="be052-163">assignments</span></span>|<span data-ttu-id="be052-164">Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be052-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="be052-165">Список назначений групп для профиля.</span><span class="sxs-lookup"><span data-stu-id="be052-165">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be052-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be052-166">JSON Representation</span></span>
<span data-ttu-id="be052-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be052-167">Here is a JSON representation of the resource.</span></span>
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
  "enableWhiteGlove": true
}
```




