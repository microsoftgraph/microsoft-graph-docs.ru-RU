---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22e71dc6a272a0e49e3ff0f60af90f63c44b3cfa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947127"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="63c98-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="63c98-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="63c98-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63c98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63c98-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63c98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63c98-106">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="63c98-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="63c98-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="63c98-107">Properties</span></span>
|<span data-ttu-id="63c98-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="63c98-108">Property</span></span>|<span data-ttu-id="63c98-109">Тип</span><span class="sxs-lookup"><span data-stu-id="63c98-109">Type</span></span>|<span data-ttu-id="63c98-110">Описание</span><span class="sxs-lookup"><span data-stu-id="63c98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63c98-111">setting</span><span class="sxs-lookup"><span data-stu-id="63c98-111">setting</span></span>|<span data-ttu-id="63c98-112">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-112">String</span></span>|<span data-ttu-id="63c98-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="63c98-113">The setting that is being reported</span></span>|
|<span data-ttu-id="63c98-114">settingName</span><span class="sxs-lookup"><span data-stu-id="63c98-114">settingName</span></span>|<span data-ttu-id="63c98-115">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-115">String</span></span>|<span data-ttu-id="63c98-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="63c98-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="63c98-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="63c98-117">instanceDisplayName</span></span>|<span data-ttu-id="63c98-118">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-118">String</span></span>|<span data-ttu-id="63c98-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="63c98-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="63c98-120">state</span><span class="sxs-lookup"><span data-stu-id="63c98-120">state</span></span>|[<span data-ttu-id="63c98-121">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="63c98-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="63c98-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="63c98-122">The compliance state of the setting.</span></span> <span data-ttu-id="63c98-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="63c98-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="63c98-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="63c98-124">errorCode</span></span>|<span data-ttu-id="63c98-125">Int64</span><span class="sxs-lookup"><span data-stu-id="63c98-125">Int64</span></span>|<span data-ttu-id="63c98-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="63c98-126">Error code for the setting</span></span>|
|<span data-ttu-id="63c98-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="63c98-127">errorDescription</span></span>|<span data-ttu-id="63c98-128">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-128">String</span></span>|<span data-ttu-id="63c98-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="63c98-129">Error description</span></span>|
|<span data-ttu-id="63c98-130">userId</span><span class="sxs-lookup"><span data-stu-id="63c98-130">userId</span></span>|<span data-ttu-id="63c98-131">String</span><span class="sxs-lookup"><span data-stu-id="63c98-131">String</span></span>|<span data-ttu-id="63c98-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="63c98-132">UserId</span></span>|
|<span data-ttu-id="63c98-133">userName</span><span class="sxs-lookup"><span data-stu-id="63c98-133">userName</span></span>|<span data-ttu-id="63c98-134">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-134">String</span></span>|<span data-ttu-id="63c98-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="63c98-135">UserName</span></span>|
|<span data-ttu-id="63c98-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="63c98-136">userEmail</span></span>|<span data-ttu-id="63c98-137">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-137">String</span></span>|<span data-ttu-id="63c98-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="63c98-138">UserEmail</span></span>|
|<span data-ttu-id="63c98-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="63c98-139">userPrincipalName</span></span>|<span data-ttu-id="63c98-140">Строка</span><span class="sxs-lookup"><span data-stu-id="63c98-140">String</span></span>|<span data-ttu-id="63c98-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="63c98-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="63c98-142">sources</span><span class="sxs-lookup"><span data-stu-id="63c98-142">sources</span></span>|<span data-ttu-id="63c98-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="63c98-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="63c98-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="63c98-144">Contributing policies</span></span>|
|<span data-ttu-id="63c98-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="63c98-145">currentValue</span></span>|<span data-ttu-id="63c98-146">String</span><span class="sxs-lookup"><span data-stu-id="63c98-146">String</span></span>|<span data-ttu-id="63c98-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="63c98-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="63c98-148">Связи</span><span class="sxs-lookup"><span data-stu-id="63c98-148">Relationships</span></span>
<span data-ttu-id="63c98-149">Нет</span><span class="sxs-lookup"><span data-stu-id="63c98-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63c98-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63c98-150">JSON Representation</span></span>
<span data-ttu-id="63c98-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63c98-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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




