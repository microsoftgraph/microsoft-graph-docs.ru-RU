---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f88561d91c4560038027245291f8a04ab270fa22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469255"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="2a0d8-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2a0d8-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="2a0d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a0d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a0d8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a0d8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a0d8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a0d8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2a0d8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a0d8-108">Properties</span></span>
|<span data-ttu-id="2a0d8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a0d8-109">Property</span></span>|<span data-ttu-id="2a0d8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2a0d8-110">Type</span></span>|<span data-ttu-id="2a0d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2a0d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a0d8-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="2a0d8-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="2a0d8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2a0d8-113">Int32</span></span>|<span data-ttu-id="2a0d8-114">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="2a0d8-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="2a0d8-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="2a0d8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0d8-116">Boolean</span></span>|<span data-ttu-id="2a0d8-117">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="2a0d8-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="2a0d8-118">secureByDefault</span></span>|<span data-ttu-id="2a0d8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0d8-119">Boolean</span></span>|<span data-ttu-id="2a0d8-120">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="2a0d8-121">енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="2a0d8-121">enhancedJailBreak</span></span>|<span data-ttu-id="2a0d8-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0d8-122">Boolean</span></span>|<span data-ttu-id="2a0d8-123">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="2a0d8-124">девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="2a0d8-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="2a0d8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2a0d8-125">Int32</span></span>|<span data-ttu-id="2a0d8-126">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="2a0d8-127">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="2a0d8-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="2a0d8-128">дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="2a0d8-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="2a0d8-129">дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="2a0d8-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="2a0d8-130">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="2a0d8-131">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="2a0d8-132">дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="2a0d8-132">derivedCredentialUrl</span></span>|<span data-ttu-id="2a0d8-133">String</span><span class="sxs-lookup"><span data-stu-id="2a0d8-133">String</span></span>|<span data-ttu-id="2a0d8-134">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="2a0d8-135">андроиддевицеадминистраторенроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="2a0d8-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="2a0d8-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0d8-136">Boolean</span></span>|<span data-ttu-id="2a0d8-137">Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|
|<span data-ttu-id="2a0d8-138">игноредевицесфорунсуппортедсеттингсенаблед</span><span class="sxs-lookup"><span data-stu-id="2a0d8-138">ignoreDevicesForUnsupportedSettingsEnabled</span></span>|<span data-ttu-id="2a0d8-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0d8-139">Boolean</span></span>|<span data-ttu-id="2a0d8-140">Свойство, определяющее, следует ли игнорировать неподдерживаемые параметры соответствия для определенных моделей устройств.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-140">The property to determine whether to ignore unsupported compliance settings on certian models of devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a0d8-141">Связи</span><span class="sxs-lookup"><span data-stu-id="2a0d8-141">Relationships</span></span>
<span data-ttu-id="2a0d8-142">Нет</span><span class="sxs-lookup"><span data-stu-id="2a0d8-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a0d8-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a0d8-143">JSON Representation</span></span>
<span data-ttu-id="2a0d8-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a0d8-144">Here is a JSON representation of the resource.</span></span>
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



