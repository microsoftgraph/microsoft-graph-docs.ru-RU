---
title: Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате
description: Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d828b57e6ae76e3a0babcc2b27a009e60f7a6407
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636299"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="b319e-103">Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате</span><span class="sxs-lookup"><span data-stu-id="b319e-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

> <span data-ttu-id="b319e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b319e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b319e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b319e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b319e-106">Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="b319e-106">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b319e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b319e-107">Properties</span></span>
|<span data-ttu-id="b319e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b319e-108">Property</span></span>|<span data-ttu-id="b319e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b319e-109">Type</span></span>|<span data-ttu-id="b319e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b319e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b319e-111">setting</span><span class="sxs-lookup"><span data-stu-id="b319e-111">setting</span></span>|<span data-ttu-id="b319e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-112">String</span></span>|<span data-ttu-id="b319e-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="b319e-113">The setting that is being reported</span></span>|
|<span data-ttu-id="b319e-114">settingName</span><span class="sxs-lookup"><span data-stu-id="b319e-114">settingName</span></span>|<span data-ttu-id="b319e-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-115">String</span></span>|<span data-ttu-id="b319e-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="b319e-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b319e-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b319e-117">instanceDisplayName</span></span>|<span data-ttu-id="b319e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-118">String</span></span>|<span data-ttu-id="b319e-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="b319e-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b319e-120">state</span><span class="sxs-lookup"><span data-stu-id="b319e-120">state</span></span>|[<span data-ttu-id="b319e-121">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="b319e-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b319e-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="b319e-122">The compliance state of the setting.</span></span> <span data-ttu-id="b319e-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b319e-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b319e-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="b319e-124">errorCode</span></span>|<span data-ttu-id="b319e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b319e-125">Int64</span></span>|<span data-ttu-id="b319e-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="b319e-126">Error code for the setting</span></span>|
|<span data-ttu-id="b319e-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b319e-127">errorDescription</span></span>|<span data-ttu-id="b319e-128">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-128">String</span></span>|<span data-ttu-id="b319e-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="b319e-129">Error description</span></span>|
|<span data-ttu-id="b319e-130">userId</span><span class="sxs-lookup"><span data-stu-id="b319e-130">userId</span></span>|<span data-ttu-id="b319e-131">String</span><span class="sxs-lookup"><span data-stu-id="b319e-131">String</span></span>|<span data-ttu-id="b319e-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="b319e-132">UserId</span></span>|
|<span data-ttu-id="b319e-133">userName</span><span class="sxs-lookup"><span data-stu-id="b319e-133">userName</span></span>|<span data-ttu-id="b319e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-134">String</span></span>|<span data-ttu-id="b319e-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b319e-135">UserName</span></span>|
|<span data-ttu-id="b319e-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="b319e-136">userEmail</span></span>|<span data-ttu-id="b319e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-137">String</span></span>|<span data-ttu-id="b319e-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="b319e-138">UserEmail</span></span>|
|<span data-ttu-id="b319e-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b319e-139">userPrincipalName</span></span>|<span data-ttu-id="b319e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b319e-140">String</span></span>|<span data-ttu-id="b319e-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b319e-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="b319e-142">sources</span><span class="sxs-lookup"><span data-stu-id="b319e-142">sources</span></span>|<span data-ttu-id="b319e-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="b319e-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b319e-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="b319e-144">Contributing policies</span></span>|
|<span data-ttu-id="b319e-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="b319e-145">currentValue</span></span>|<span data-ttu-id="b319e-146">String</span><span class="sxs-lookup"><span data-stu-id="b319e-146">String</span></span>|<span data-ttu-id="b319e-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="b319e-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b319e-148">Связи</span><span class="sxs-lookup"><span data-stu-id="b319e-148">Relationships</span></span>
<span data-ttu-id="b319e-149">Нет</span><span class="sxs-lookup"><span data-stu-id="b319e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b319e-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b319e-150">JSON Representation</span></span>
<span data-ttu-id="b319e-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b319e-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



