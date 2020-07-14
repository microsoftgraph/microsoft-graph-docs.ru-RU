---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7dd44406211e8d0763625e5c1ae252444505265e
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123955"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="71392-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="71392-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="71392-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71392-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71392-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71392-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71392-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71392-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71392-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="71392-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="71392-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="71392-108">Properties</span></span>
|<span data-ttu-id="71392-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="71392-109">Property</span></span>|<span data-ttu-id="71392-110">Тип</span><span class="sxs-lookup"><span data-stu-id="71392-110">Type</span></span>|<span data-ttu-id="71392-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71392-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71392-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="71392-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="71392-113">Int32</span><span class="sxs-lookup"><span data-stu-id="71392-113">Int32</span></span>|<span data-ttu-id="71392-114">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="71392-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="71392-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="71392-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="71392-116">Логический</span><span class="sxs-lookup"><span data-stu-id="71392-116">Boolean</span></span>|<span data-ttu-id="71392-117">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="71392-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="71392-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="71392-118">secureByDefault</span></span>|<span data-ttu-id="71392-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="71392-119">Boolean</span></span>|<span data-ttu-id="71392-120">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="71392-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="71392-121">енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="71392-121">enhancedJailBreak</span></span>|<span data-ttu-id="71392-122">Логический</span><span class="sxs-lookup"><span data-stu-id="71392-122">Boolean</span></span>|<span data-ttu-id="71392-123">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="71392-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="71392-124">девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="71392-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="71392-125">Int32</span><span class="sxs-lookup"><span data-stu-id="71392-125">Int32</span></span>|<span data-ttu-id="71392-126">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="71392-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="71392-127">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="71392-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="71392-128">дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="71392-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="71392-129">дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="71392-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="71392-130">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="71392-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="71392-131">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="71392-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="71392-132">дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="71392-132">derivedCredentialUrl</span></span>|<span data-ttu-id="71392-133">String</span><span class="sxs-lookup"><span data-stu-id="71392-133">String</span></span>|<span data-ttu-id="71392-134">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="71392-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="71392-135">андроиддевицеадминистраторенроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="71392-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="71392-136">Логический</span><span class="sxs-lookup"><span data-stu-id="71392-136">Boolean</span></span>|<span data-ttu-id="71392-137">Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="71392-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|
|<span data-ttu-id="71392-138">игноредевицесфорунсуппортедсеттингсенаблед</span><span class="sxs-lookup"><span data-stu-id="71392-138">ignoreDevicesForUnsupportedSettingsEnabled</span></span>|<span data-ttu-id="71392-139">Логический</span><span class="sxs-lookup"><span data-stu-id="71392-139">Boolean</span></span>|<span data-ttu-id="71392-140">Свойство, определяющее, следует ли игнорировать неподдерживаемые параметры соответствия для определенных моделей устройств.</span><span class="sxs-lookup"><span data-stu-id="71392-140">The property to determine whether to ignore unsupported compliance settings on certian models of devices.</span></span>|
|<span data-ttu-id="71392-141">енаблелогколлектион</span><span class="sxs-lookup"><span data-stu-id="71392-141">enableLogCollection</span></span>|<span data-ttu-id="71392-142">Логический</span><span class="sxs-lookup"><span data-stu-id="71392-142">Boolean</span></span>|<span data-ttu-id="71392-143">Определяет, доступна ли функция сбора журналов для использования.</span><span class="sxs-lookup"><span data-stu-id="71392-143">Determines whether the log collection feature should be available for use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71392-144">Связи</span><span class="sxs-lookup"><span data-stu-id="71392-144">Relationships</span></span>
<span data-ttu-id="71392-145">Нет</span><span class="sxs-lookup"><span data-stu-id="71392-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71392-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71392-146">JSON Representation</span></span>
<span data-ttu-id="71392-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71392-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true,
  "enableLogCollection": true
}
```



