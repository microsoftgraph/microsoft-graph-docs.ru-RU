---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdc01e2c9cd4aabf47c900bd38bb2b0f7035308b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538968"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="189f0-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="189f0-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="189f0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="189f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="189f0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="189f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="189f0-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="189f0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="189f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="189f0-107">Properties</span></span>
|<span data-ttu-id="189f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="189f0-108">Property</span></span>|<span data-ttu-id="189f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="189f0-109">Type</span></span>|<span data-ttu-id="189f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="189f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="189f0-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="189f0-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="189f0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="189f0-112">Int32</span></span>|<span data-ttu-id="189f0-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="189f0-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="189f0-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="189f0-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="189f0-115">Логический</span><span class="sxs-lookup"><span data-stu-id="189f0-115">Boolean</span></span>|<span data-ttu-id="189f0-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="189f0-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="189f0-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="189f0-117">secureByDefault</span></span>|<span data-ttu-id="189f0-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="189f0-118">Boolean</span></span>|<span data-ttu-id="189f0-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="189f0-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="189f0-120">енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="189f0-120">enhancedJailBreak</span></span>|<span data-ttu-id="189f0-121">Логический</span><span class="sxs-lookup"><span data-stu-id="189f0-121">Boolean</span></span>|<span data-ttu-id="189f0-122">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="189f0-122">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="189f0-123">девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="189f0-123">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="189f0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="189f0-124">Int32</span></span>|<span data-ttu-id="189f0-125">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="189f0-125">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="189f0-126">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="189f0-126">Valid values 30 to 270</span></span>|
|<span data-ttu-id="189f0-127">дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="189f0-127">derivedCredentialProvider</span></span>|[<span data-ttu-id="189f0-128">дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="189f0-128">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="189f0-129">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="189f0-129">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="189f0-130">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="189f0-130">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="189f0-131">дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="189f0-131">derivedCredentialUrl</span></span>|<span data-ttu-id="189f0-132">String</span><span class="sxs-lookup"><span data-stu-id="189f0-132">String</span></span>|<span data-ttu-id="189f0-133">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="189f0-133">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="189f0-134">андроиддевицеадминистраторенроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="189f0-134">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="189f0-135">Логический</span><span class="sxs-lookup"><span data-stu-id="189f0-135">Boolean</span></span>|<span data-ttu-id="189f0-136">Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="189f0-136">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="189f0-137">Связи</span><span class="sxs-lookup"><span data-stu-id="189f0-137">Relationships</span></span>
<span data-ttu-id="189f0-138">Нет</span><span class="sxs-lookup"><span data-stu-id="189f0-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="189f0-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="189f0-139">JSON Representation</span></span>
<span data-ttu-id="189f0-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="189f0-140">Here is a JSON representation of the resource.</span></span>
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
  "androidDeviceAdministratorEnrollmentEnabled": true
}
```



