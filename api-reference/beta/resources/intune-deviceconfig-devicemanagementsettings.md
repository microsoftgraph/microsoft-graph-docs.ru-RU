---
title: Тип ресурса deviceManagementSettings
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f676eed1acbf6711f526e612bd6c073b749607d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417667"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="a60bd-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="a60bd-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="a60bd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a60bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a60bd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a60bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a60bd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a60bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a60bd-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a60bd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a60bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a60bd-108">Properties</span></span>
|<span data-ttu-id="a60bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a60bd-109">Property</span></span>|<span data-ttu-id="a60bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a60bd-110">Type</span></span>|<span data-ttu-id="a60bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a60bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a60bd-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a60bd-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="a60bd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a60bd-113">Int32</span></span>|<span data-ttu-id="a60bd-114">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="a60bd-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="a60bd-115">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="a60bd-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="a60bd-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="a60bd-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="a60bd-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a60bd-117">Boolean</span></span>|<span data-ttu-id="a60bd-118">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="a60bd-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="a60bd-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="a60bd-119">secureByDefault</span></span>|<span data-ttu-id="a60bd-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a60bd-120">Boolean</span></span>|<span data-ttu-id="a60bd-121">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="a60bd-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="a60bd-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="a60bd-122">enhancedJailBreak</span></span>|<span data-ttu-id="a60bd-123">Логический</span><span class="sxs-lookup"><span data-stu-id="a60bd-123">Boolean</span></span>|<span data-ttu-id="a60bd-124">— Это функция включена или не для улучшения обнаружения jailbreak.</span><span class="sxs-lookup"><span data-stu-id="a60bd-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="a60bd-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="a60bd-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="a60bd-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a60bd-126">Int32</span></span>|<span data-ttu-id="a60bd-127">Когда устройство не проверяет, для указанного числа дней, компании данных может быть удален, устройство не будет в разделе Управление.</span><span class="sxs-lookup"><span data-stu-id="a60bd-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="a60bd-128">Допустимые значения 30 на 270 градусов</span><span class="sxs-lookup"><span data-stu-id="a60bd-128">Valid values 30 to 270</span></span>|
|<span data-ttu-id="a60bd-129">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="a60bd-129">derivedCredentialProvider</span></span>|[<span data-ttu-id="a60bd-130">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="a60bd-130">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="a60bd-131">Производные поставщик учетных данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a60bd-131">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="a60bd-132">Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="a60bd-132">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="a60bd-133">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="a60bd-133">derivedCredentialUrl</span></span>|<span data-ttu-id="a60bd-134">String</span><span class="sxs-lookup"><span data-stu-id="a60bd-134">String</span></span>|<span data-ttu-id="a60bd-135">URI самостоятельного производные поставщика учетных данных.</span><span class="sxs-lookup"><span data-stu-id="a60bd-135">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a60bd-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="a60bd-136">Relationships</span></span>
<span data-ttu-id="a60bd-137">Нет</span><span class="sxs-lookup"><span data-stu-id="a60bd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a60bd-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a60bd-138">JSON Representation</span></span>
<span data-ttu-id="a60bd-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a60bd-139">Here is a JSON representation of the resource.</span></span>
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




