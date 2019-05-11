---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 079d957d14e5f891af691ba7b41916adb8ac9669
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946968"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="64d3b-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="64d3b-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="64d3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64d3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64d3b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64d3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64d3b-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="64d3b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="64d3b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="64d3b-107">Properties</span></span>
|<span data-ttu-id="64d3b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="64d3b-108">Property</span></span>|<span data-ttu-id="64d3b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="64d3b-109">Type</span></span>|<span data-ttu-id="64d3b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64d3b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64d3b-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="64d3b-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="64d3b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="64d3b-112">Int32</span></span>|<span data-ttu-id="64d3b-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="64d3b-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="64d3b-114">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="64d3b-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="64d3b-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="64d3b-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="64d3b-116">Логический</span><span class="sxs-lookup"><span data-stu-id="64d3b-116">Boolean</span></span>|<span data-ttu-id="64d3b-117">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="64d3b-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="64d3b-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="64d3b-118">secureByDefault</span></span>|<span data-ttu-id="64d3b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="64d3b-119">Boolean</span></span>|<span data-ttu-id="64d3b-120">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="64d3b-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="64d3b-121">Енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="64d3b-121">enhancedJailBreak</span></span>|<span data-ttu-id="64d3b-122">Логический</span><span class="sxs-lookup"><span data-stu-id="64d3b-122">Boolean</span></span>|<span data-ttu-id="64d3b-123">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="64d3b-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="64d3b-124">Девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="64d3b-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="64d3b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="64d3b-125">Int32</span></span>|<span data-ttu-id="64d3b-126">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="64d3b-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="64d3b-127">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="64d3b-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="64d3b-128">Дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="64d3b-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="64d3b-129">Дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="64d3b-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="64d3b-130">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="64d3b-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="64d3b-131">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="64d3b-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="64d3b-132">Дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="64d3b-132">derivedCredentialUrl</span></span>|<span data-ttu-id="64d3b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="64d3b-133">String</span></span>|<span data-ttu-id="64d3b-134">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="64d3b-134">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64d3b-135">Связи</span><span class="sxs-lookup"><span data-stu-id="64d3b-135">Relationships</span></span>
<span data-ttu-id="64d3b-136">Нет</span><span class="sxs-lookup"><span data-stu-id="64d3b-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64d3b-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64d3b-137">JSON Representation</span></span>
<span data-ttu-id="64d3b-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64d3b-138">Here is a JSON representation of the resource.</span></span>
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
  "derivedCredentialUrl": "String"
}
```




