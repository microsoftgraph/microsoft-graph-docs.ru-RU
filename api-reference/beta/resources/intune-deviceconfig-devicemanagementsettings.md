---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4be3b818ec414d99af677965ed7324d8b52a9099
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004549"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="1806f-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="1806f-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="1806f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1806f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1806f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1806f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1806f-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1806f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1806f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1806f-107">Properties</span></span>
|<span data-ttu-id="1806f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1806f-108">Property</span></span>|<span data-ttu-id="1806f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1806f-109">Type</span></span>|<span data-ttu-id="1806f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1806f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1806f-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="1806f-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="1806f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1806f-112">Int32</span></span>|<span data-ttu-id="1806f-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="1806f-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="1806f-114">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="1806f-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="1806f-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="1806f-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="1806f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1806f-116">Boolean</span></span>|<span data-ttu-id="1806f-117">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="1806f-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="1806f-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="1806f-118">secureByDefault</span></span>|<span data-ttu-id="1806f-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1806f-119">Boolean</span></span>|<span data-ttu-id="1806f-120">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="1806f-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="1806f-121">Енханцеджаилбреак</span><span class="sxs-lookup"><span data-stu-id="1806f-121">enhancedJailBreak</span></span>|<span data-ttu-id="1806f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1806f-122">Boolean</span></span>|<span data-ttu-id="1806f-123">Функция включена или не включена для обнаружения расширенной жаилбреак.</span><span class="sxs-lookup"><span data-stu-id="1806f-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="1806f-124">Девицеинактивитибефореретирементиндай</span><span class="sxs-lookup"><span data-stu-id="1806f-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="1806f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1806f-125">Int32</span></span>|<span data-ttu-id="1806f-126">Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться.</span><span class="sxs-lookup"><span data-stu-id="1806f-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="1806f-127">Допустимые значения — от 30 до 270</span><span class="sxs-lookup"><span data-stu-id="1806f-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="1806f-128">Дериведкредентиалпровидер</span><span class="sxs-lookup"><span data-stu-id="1806f-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="1806f-129">Дериведкредентиалпровидертипе</span><span class="sxs-lookup"><span data-stu-id="1806f-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="1806f-130">Производный поставщик учетных данных, который будет использоваться для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="1806f-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="1806f-131">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="1806f-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="1806f-132">Дериведкредентиалурл</span><span class="sxs-lookup"><span data-stu-id="1806f-132">derivedCredentialUrl</span></span>|<span data-ttu-id="1806f-133">String</span><span class="sxs-lookup"><span data-stu-id="1806f-133">String</span></span>|<span data-ttu-id="1806f-134">URI самообслуживания поставщика производных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="1806f-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="1806f-135">Андроиддевицеадминистраторенроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="1806f-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="1806f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="1806f-136">Boolean</span></span>|<span data-ttu-id="1806f-137">Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="1806f-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1806f-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="1806f-138">Relationships</span></span>
<span data-ttu-id="1806f-139">Нет</span><span class="sxs-lookup"><span data-stu-id="1806f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1806f-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1806f-140">JSON Representation</span></span>
<span data-ttu-id="1806f-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1806f-141">Here is a JSON representation of the resource.</span></span>
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





