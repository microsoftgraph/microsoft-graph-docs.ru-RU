---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b3e622c5231bd985a6834e9b6b1d908860385245
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792012"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="fe766-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="fe766-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="fe766-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe766-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe766-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe766-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe766-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fe766-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fe766-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe766-107">Properties</span></span>
|<span data-ttu-id="fe766-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe766-108">Property</span></span>|<span data-ttu-id="fe766-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fe766-109">Type</span></span>|<span data-ttu-id="fe766-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe766-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe766-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="fe766-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="fe766-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fe766-112">Int32</span></span>|<span data-ttu-id="fe766-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="fe766-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="fe766-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="fe766-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="fe766-115">Логический</span><span class="sxs-lookup"><span data-stu-id="fe766-115">Boolean</span></span>|<span data-ttu-id="fe766-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="fe766-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="fe766-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="fe766-117">secureByDefault</span></span>|<span data-ttu-id="fe766-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe766-118">Boolean</span></span>|<span data-ttu-id="fe766-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="fe766-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="fe766-120">енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="fe766-120">enhancedJailBreak</span></span>|<span data-ttu-id="fe766-121">Логический</span><span class="sxs-lookup"><span data-stu-id="fe766-121">Boolean</span></span>|<span data-ttu-id="fe766-122">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="fe766-122">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="fe766-123">девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="fe766-123">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="fe766-124">Int32</span><span class="sxs-lookup"><span data-stu-id="fe766-124">Int32</span></span>|<span data-ttu-id="fe766-125">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="fe766-125">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="fe766-126">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="fe766-126">Valid values 30 to 270</span></span>|
|<span data-ttu-id="fe766-127">дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="fe766-127">derivedCredentialProvider</span></span>|[<span data-ttu-id="fe766-128">дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="fe766-128">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="fe766-129">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="fe766-129">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="fe766-130">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="fe766-130">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="fe766-131">дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="fe766-131">derivedCredentialUrl</span></span>|<span data-ttu-id="fe766-132">String</span><span class="sxs-lookup"><span data-stu-id="fe766-132">String</span></span>|<span data-ttu-id="fe766-133">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="fe766-133">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="fe766-134">андроиддевицеадминистраторенроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="fe766-134">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="fe766-135">Логический</span><span class="sxs-lookup"><span data-stu-id="fe766-135">Boolean</span></span>|<span data-ttu-id="fe766-136">Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="fe766-136">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|
|<span data-ttu-id="fe766-137">игноредевицесфорунсуппортедсеттингсенаблед</span><span class="sxs-lookup"><span data-stu-id="fe766-137">ignoreDevicesForUnsupportedSettingsEnabled</span></span>|<span data-ttu-id="fe766-138">Логический</span><span class="sxs-lookup"><span data-stu-id="fe766-138">Boolean</span></span>|<span data-ttu-id="fe766-139">Свойство, определяющее, следует ли игнорировать неподдерживаемые параметры соответствия для определенных моделей устройств.</span><span class="sxs-lookup"><span data-stu-id="fe766-139">The property to determine whether to ignore unsupported compliance settings on certian models of devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe766-140">Связи</span><span class="sxs-lookup"><span data-stu-id="fe766-140">Relationships</span></span>
<span data-ttu-id="fe766-141">Нет</span><span class="sxs-lookup"><span data-stu-id="fe766-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe766-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe766-142">JSON Representation</span></span>
<span data-ttu-id="fe766-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe766-143">Here is a JSON representation of the resource.</span></span>
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
  "ignoreDevicesForUnsupportedSettingsEnabled": true
}
```



