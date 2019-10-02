---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e26beda0907c8a8e56c202088dfaad666b795ee7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359623"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="b53eb-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="b53eb-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="b53eb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b53eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b53eb-105">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="b53eb-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b53eb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b53eb-106">Properties</span></span>
|<span data-ttu-id="b53eb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b53eb-107">Property</span></span>|<span data-ttu-id="b53eb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b53eb-108">Type</span></span>|<span data-ttu-id="b53eb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b53eb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b53eb-110">setting</span><span class="sxs-lookup"><span data-stu-id="b53eb-110">setting</span></span>|<span data-ttu-id="b53eb-111">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-111">String</span></span>|<span data-ttu-id="b53eb-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="b53eb-112">The setting that is being reported</span></span>|
|<span data-ttu-id="b53eb-113">settingName</span><span class="sxs-lookup"><span data-stu-id="b53eb-113">settingName</span></span>|<span data-ttu-id="b53eb-114">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-114">String</span></span>|<span data-ttu-id="b53eb-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="b53eb-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b53eb-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b53eb-116">instanceDisplayName</span></span>|<span data-ttu-id="b53eb-117">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-117">String</span></span>|<span data-ttu-id="b53eb-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="b53eb-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b53eb-119">state</span><span class="sxs-lookup"><span data-stu-id="b53eb-119">state</span></span>|[<span data-ttu-id="b53eb-120">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="b53eb-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b53eb-121">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="b53eb-121">The compliance state of the setting.</span></span> <span data-ttu-id="b53eb-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b53eb-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b53eb-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="b53eb-123">errorCode</span></span>|<span data-ttu-id="b53eb-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b53eb-124">Int64</span></span>|<span data-ttu-id="b53eb-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="b53eb-125">Error code for the setting</span></span>|
|<span data-ttu-id="b53eb-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b53eb-126">errorDescription</span></span>|<span data-ttu-id="b53eb-127">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-127">String</span></span>|<span data-ttu-id="b53eb-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="b53eb-128">Error description</span></span>|
|<span data-ttu-id="b53eb-129">userId</span><span class="sxs-lookup"><span data-stu-id="b53eb-129">userId</span></span>|<span data-ttu-id="b53eb-130">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-130">String</span></span>|<span data-ttu-id="b53eb-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="b53eb-131">UserId</span></span>|
|<span data-ttu-id="b53eb-132">userName</span><span class="sxs-lookup"><span data-stu-id="b53eb-132">userName</span></span>|<span data-ttu-id="b53eb-133">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-133">String</span></span>|<span data-ttu-id="b53eb-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b53eb-134">UserName</span></span>|
|<span data-ttu-id="b53eb-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="b53eb-135">userEmail</span></span>|<span data-ttu-id="b53eb-136">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-136">String</span></span>|<span data-ttu-id="b53eb-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="b53eb-137">UserEmail</span></span>|
|<span data-ttu-id="b53eb-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b53eb-138">userPrincipalName</span></span>|<span data-ttu-id="b53eb-139">Строка</span><span class="sxs-lookup"><span data-stu-id="b53eb-139">String</span></span>|<span data-ttu-id="b53eb-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b53eb-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="b53eb-141">sources</span><span class="sxs-lookup"><span data-stu-id="b53eb-141">sources</span></span>|<span data-ttu-id="b53eb-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="b53eb-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b53eb-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="b53eb-143">Contributing policies</span></span>|
|<span data-ttu-id="b53eb-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="b53eb-144">currentValue</span></span>|<span data-ttu-id="b53eb-145">String</span><span class="sxs-lookup"><span data-stu-id="b53eb-145">String</span></span>|<span data-ttu-id="b53eb-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="b53eb-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b53eb-147">Связи</span><span class="sxs-lookup"><span data-stu-id="b53eb-147">Relationships</span></span>
<span data-ttu-id="b53eb-148">Нет</span><span class="sxs-lookup"><span data-stu-id="b53eb-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b53eb-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b53eb-149">JSON Representation</span></span>
<span data-ttu-id="b53eb-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b53eb-150">Here is a JSON representation of the resource.</span></span>
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




