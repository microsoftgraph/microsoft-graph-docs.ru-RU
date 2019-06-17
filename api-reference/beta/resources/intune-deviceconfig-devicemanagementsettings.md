---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a087192b9ff46b79f5f585cc9515b9c78d806e99
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990010"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="31214-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="31214-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="31214-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31214-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31214-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31214-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31214-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="31214-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="31214-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="31214-107">Properties</span></span>
|<span data-ttu-id="31214-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="31214-108">Property</span></span>|<span data-ttu-id="31214-109">Тип</span><span class="sxs-lookup"><span data-stu-id="31214-109">Type</span></span>|<span data-ttu-id="31214-110">Описание</span><span class="sxs-lookup"><span data-stu-id="31214-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31214-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="31214-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="31214-112">Int32</span><span class="sxs-lookup"><span data-stu-id="31214-112">Int32</span></span>|<span data-ttu-id="31214-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="31214-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="31214-114">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="31214-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="31214-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="31214-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="31214-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="31214-116">Boolean</span></span>|<span data-ttu-id="31214-117">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="31214-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="31214-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="31214-118">secureByDefault</span></span>|<span data-ttu-id="31214-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="31214-119">Boolean</span></span>|<span data-ttu-id="31214-120">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="31214-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="31214-121">Енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="31214-121">enhancedJailBreak</span></span>|<span data-ttu-id="31214-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="31214-122">Boolean</span></span>|<span data-ttu-id="31214-123">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="31214-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="31214-124">Девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="31214-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="31214-125">Int32</span><span class="sxs-lookup"><span data-stu-id="31214-125">Int32</span></span>|<span data-ttu-id="31214-126">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="31214-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="31214-127">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="31214-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="31214-128">Дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="31214-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="31214-129">Дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="31214-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="31214-130">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="31214-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="31214-131">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="31214-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="31214-132">Дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="31214-132">derivedCredentialUrl</span></span>|<span data-ttu-id="31214-133">String</span><span class="sxs-lookup"><span data-stu-id="31214-133">String</span></span>|<span data-ttu-id="31214-134">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="31214-134">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31214-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="31214-135">Relationships</span></span>
<span data-ttu-id="31214-136">Нет</span><span class="sxs-lookup"><span data-stu-id="31214-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31214-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31214-137">JSON Representation</span></span>
<span data-ttu-id="31214-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31214-138">Here is a JSON representation of the resource.</span></span>
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





