---
title: Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате
description: Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 740d2fe591810829080ed6da78e9c6fcc68e7d52
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788620"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="c63a8-103">Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате</span><span class="sxs-lookup"><span data-stu-id="c63a8-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

> <span data-ttu-id="c63a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c63a8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c63a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63a8-106">Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="c63a8-106">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="c63a8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c63a8-107">Properties</span></span>
|<span data-ttu-id="c63a8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c63a8-108">Property</span></span>|<span data-ttu-id="c63a8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c63a8-109">Type</span></span>|<span data-ttu-id="c63a8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c63a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63a8-111">setting</span><span class="sxs-lookup"><span data-stu-id="c63a8-111">setting</span></span>|<span data-ttu-id="c63a8-112">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-112">String</span></span>|<span data-ttu-id="c63a8-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="c63a8-113">The setting that is being reported</span></span>|
|<span data-ttu-id="c63a8-114">settingName</span><span class="sxs-lookup"><span data-stu-id="c63a8-114">settingName</span></span>|<span data-ttu-id="c63a8-115">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-115">String</span></span>|<span data-ttu-id="c63a8-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="c63a8-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="c63a8-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c63a8-117">instanceDisplayName</span></span>|<span data-ttu-id="c63a8-118">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-118">String</span></span>|<span data-ttu-id="c63a8-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="c63a8-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="c63a8-120">state</span><span class="sxs-lookup"><span data-stu-id="c63a8-120">state</span></span>|[<span data-ttu-id="c63a8-121">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="c63a8-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c63a8-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="c63a8-122">The compliance state of the setting.</span></span> <span data-ttu-id="c63a8-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c63a8-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c63a8-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="c63a8-124">errorCode</span></span>|<span data-ttu-id="c63a8-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c63a8-125">Int64</span></span>|<span data-ttu-id="c63a8-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="c63a8-126">Error code for the setting</span></span>|
|<span data-ttu-id="c63a8-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="c63a8-127">errorDescription</span></span>|<span data-ttu-id="c63a8-128">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-128">String</span></span>|<span data-ttu-id="c63a8-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="c63a8-129">Error description</span></span>|
|<span data-ttu-id="c63a8-130">userId</span><span class="sxs-lookup"><span data-stu-id="c63a8-130">userId</span></span>|<span data-ttu-id="c63a8-131">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-131">String</span></span>|<span data-ttu-id="c63a8-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="c63a8-132">UserId</span></span>|
|<span data-ttu-id="c63a8-133">userName</span><span class="sxs-lookup"><span data-stu-id="c63a8-133">userName</span></span>|<span data-ttu-id="c63a8-134">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-134">String</span></span>|<span data-ttu-id="c63a8-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="c63a8-135">UserName</span></span>|
|<span data-ttu-id="c63a8-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="c63a8-136">userEmail</span></span>|<span data-ttu-id="c63a8-137">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-137">String</span></span>|<span data-ttu-id="c63a8-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="c63a8-138">UserEmail</span></span>|
|<span data-ttu-id="c63a8-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c63a8-139">userPrincipalName</span></span>|<span data-ttu-id="c63a8-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c63a8-140">String</span></span>|<span data-ttu-id="c63a8-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="c63a8-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="c63a8-142">sources</span><span class="sxs-lookup"><span data-stu-id="c63a8-142">sources</span></span>|<span data-ttu-id="c63a8-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="c63a8-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="c63a8-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="c63a8-144">Contributing policies</span></span>|
|<span data-ttu-id="c63a8-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="c63a8-145">currentValue</span></span>|<span data-ttu-id="c63a8-146">String</span><span class="sxs-lookup"><span data-stu-id="c63a8-146">String</span></span>|<span data-ttu-id="c63a8-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="c63a8-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="c63a8-148">Связи</span><span class="sxs-lookup"><span data-stu-id="c63a8-148">Relationships</span></span>
<span data-ttu-id="c63a8-149">Нет</span><span class="sxs-lookup"><span data-stu-id="c63a8-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c63a8-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c63a8-150">JSON Representation</span></span>
<span data-ttu-id="c63a8-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c63a8-151">Here is a JSON representation of the resource.</span></span>
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



