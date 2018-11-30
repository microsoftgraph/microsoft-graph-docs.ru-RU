---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Windows автопилот развертывания профилей
ms.openlocfilehash: ed109af370d73d22d46198b206ba42dc4ebab2da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076179"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="54947-103">Тип ресурса windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="54947-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="54947-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54947-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54947-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54947-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54947-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54947-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54947-107">Windows автопилот развертывания профилей</span><span class="sxs-lookup"><span data-stu-id="54947-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="54947-108">Методы</span><span class="sxs-lookup"><span data-stu-id="54947-108">Methods</span></span>
|<span data-ttu-id="54947-109">Метод</span><span class="sxs-lookup"><span data-stu-id="54947-109">Method</span></span>|<span data-ttu-id="54947-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="54947-110">Return Type</span></span>|<span data-ttu-id="54947-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54947-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54947-112">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="54947-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="54947-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="54947-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="54947-114">Чтение свойства и связи объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="54947-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="54947-115">Действие assign</span><span class="sxs-lookup"><span data-stu-id="54947-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="54947-116">Нет</span><span class="sxs-lookup"><span data-stu-id="54947-116">None</span></span>|<span data-ttu-id="54947-117">Н/Д</span><span class="sxs-lookup"><span data-stu-id="54947-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="54947-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="54947-118">Properties</span></span>
|<span data-ttu-id="54947-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="54947-119">Property</span></span>|<span data-ttu-id="54947-120">Тип</span><span class="sxs-lookup"><span data-stu-id="54947-120">Type</span></span>|<span data-ttu-id="54947-121">Описание</span><span class="sxs-lookup"><span data-stu-id="54947-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54947-122">id</span><span class="sxs-lookup"><span data-stu-id="54947-122">id</span></span>|<span data-ttu-id="54947-123">String</span><span class="sxs-lookup"><span data-stu-id="54947-123">String</span></span>|<span data-ttu-id="54947-124">Клавиша профилей</span><span class="sxs-lookup"><span data-stu-id="54947-124">Profile Key</span></span>|
|<span data-ttu-id="54947-125">displayName</span><span class="sxs-lookup"><span data-stu-id="54947-125">displayName</span></span>|<span data-ttu-id="54947-126">String</span><span class="sxs-lookup"><span data-stu-id="54947-126">String</span></span>|<span data-ttu-id="54947-127">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="54947-127">Name of the profile</span></span>|
|<span data-ttu-id="54947-128">описание</span><span class="sxs-lookup"><span data-stu-id="54947-128">description</span></span>|<span data-ttu-id="54947-129">String</span><span class="sxs-lookup"><span data-stu-id="54947-129">String</span></span>|<span data-ttu-id="54947-130">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="54947-130">Description of the profile</span></span>|
|<span data-ttu-id="54947-131">language</span><span class="sxs-lookup"><span data-stu-id="54947-131">language</span></span>|<span data-ttu-id="54947-132">String</span><span class="sxs-lookup"><span data-stu-id="54947-132">String</span></span>|<span data-ttu-id="54947-133">Язык, настроенных на устройстве</span><span class="sxs-lookup"><span data-stu-id="54947-133">Language configured on the device</span></span>|
|<span data-ttu-id="54947-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54947-134">createdDateTime</span></span>|<span data-ttu-id="54947-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54947-135">DateTimeOffset</span></span>|<span data-ttu-id="54947-136">Время создания профилей</span><span class="sxs-lookup"><span data-stu-id="54947-136">Profile creation time</span></span>|
|<span data-ttu-id="54947-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54947-137">lastModifiedDateTime</span></span>|<span data-ttu-id="54947-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54947-138">DateTimeOffset</span></span>|<span data-ttu-id="54947-139">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="54947-139">Profile last modified time</span></span>|
|<span data-ttu-id="54947-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="54947-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="54947-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="54947-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="54947-142">В соответствующем взаимодействия параметр</span><span class="sxs-lookup"><span data-stu-id="54947-142">Out of box experience setting</span></span>|
|<span data-ttu-id="54947-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="54947-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="54947-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="54947-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="54947-145">Параметр экрана состояния подачи заявок</span><span class="sxs-lookup"><span data-stu-id="54947-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="54947-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="54947-146">extractHardwareHash</span></span>|<span data-ttu-id="54947-147">Логический</span><span class="sxs-lookup"><span data-stu-id="54947-147">Boolean</span></span>|<span data-ttu-id="54947-148">Извлечение HardwareHash для профиля</span><span class="sxs-lookup"><span data-stu-id="54947-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="54947-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="54947-149">deviceNameTemplate</span></span>|<span data-ttu-id="54947-150">String</span><span class="sxs-lookup"><span data-stu-id="54947-150">String</span></span>|<span data-ttu-id="54947-151">Шаблон, используемый для имя устройства автопилот.</span><span class="sxs-lookup"><span data-stu-id="54947-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="54947-152">Это может быть настраиваемого текста, а также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="54947-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="54947-153">Общая длина текста, созданной с помощью шаблона может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="54947-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54947-154">Связи</span><span class="sxs-lookup"><span data-stu-id="54947-154">Relationships</span></span>
|<span data-ttu-id="54947-155">Связь</span><span class="sxs-lookup"><span data-stu-id="54947-155">Relationship</span></span>|<span data-ttu-id="54947-156">Тип</span><span class="sxs-lookup"><span data-stu-id="54947-156">Type</span></span>|<span data-ttu-id="54947-157">Description</span><span class="sxs-lookup"><span data-stu-id="54947-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54947-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="54947-158">assignedDevices</span></span>|<span data-ttu-id="54947-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="54947-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="54947-160">Список устройств, назначенных для профиля.</span><span class="sxs-lookup"><span data-stu-id="54947-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="54947-161">assignments</span><span class="sxs-lookup"><span data-stu-id="54947-161">assignments</span></span>|<span data-ttu-id="54947-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="54947-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="54947-163">Список назначений группы для профиля.</span><span class="sxs-lookup"><span data-stu-id="54947-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54947-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54947-164">JSON Representation</span></span>
<span data-ttu-id="54947-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54947-165">Here is a JSON representation of the resource.</span></span>
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





