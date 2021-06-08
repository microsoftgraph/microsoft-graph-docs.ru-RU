---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a7bdee8183ad86306234b446813c9272137113d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760115"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="d8fba-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="d8fba-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="d8fba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8fba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8fba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8fba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8fba-106">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="d8fba-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="d8fba-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8fba-107">Properties</span></span>
|<span data-ttu-id="d8fba-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8fba-108">Property</span></span>|<span data-ttu-id="d8fba-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d8fba-109">Type</span></span>|<span data-ttu-id="d8fba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8fba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8fba-111">setting</span><span class="sxs-lookup"><span data-stu-id="d8fba-111">setting</span></span>|<span data-ttu-id="d8fba-112">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-112">String</span></span>|<span data-ttu-id="d8fba-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="d8fba-113">The setting that is being reported</span></span>|
|<span data-ttu-id="d8fba-114">settingName</span><span class="sxs-lookup"><span data-stu-id="d8fba-114">settingName</span></span>|<span data-ttu-id="d8fba-115">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-115">String</span></span>|<span data-ttu-id="d8fba-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="d8fba-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="d8fba-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8fba-117">instanceDisplayName</span></span>|<span data-ttu-id="d8fba-118">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-118">String</span></span>|<span data-ttu-id="d8fba-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="d8fba-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="d8fba-120">state</span><span class="sxs-lookup"><span data-stu-id="d8fba-120">state</span></span>|[<span data-ttu-id="d8fba-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d8fba-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d8fba-122">Состояние соответствия параметру.</span><span class="sxs-lookup"><span data-stu-id="d8fba-122">The compliance state of the setting.</span></span> <span data-ttu-id="d8fba-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d8fba-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d8fba-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="d8fba-124">errorCode</span></span>|<span data-ttu-id="d8fba-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d8fba-125">Int64</span></span>|<span data-ttu-id="d8fba-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="d8fba-126">Error code for the setting</span></span>|
|<span data-ttu-id="d8fba-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="d8fba-127">errorDescription</span></span>|<span data-ttu-id="d8fba-128">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-128">String</span></span>|<span data-ttu-id="d8fba-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="d8fba-129">Error description</span></span>|
|<span data-ttu-id="d8fba-130">userId</span><span class="sxs-lookup"><span data-stu-id="d8fba-130">userId</span></span>|<span data-ttu-id="d8fba-131">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-131">String</span></span>|<span data-ttu-id="d8fba-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="d8fba-132">UserId</span></span>|
|<span data-ttu-id="d8fba-133">userName</span><span class="sxs-lookup"><span data-stu-id="d8fba-133">userName</span></span>|<span data-ttu-id="d8fba-134">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-134">String</span></span>|<span data-ttu-id="d8fba-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="d8fba-135">UserName</span></span>|
|<span data-ttu-id="d8fba-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="d8fba-136">userEmail</span></span>|<span data-ttu-id="d8fba-137">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-137">String</span></span>|<span data-ttu-id="d8fba-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="d8fba-138">UserEmail</span></span>|
|<span data-ttu-id="d8fba-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8fba-139">userPrincipalName</span></span>|<span data-ttu-id="d8fba-140">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-140">String</span></span>|<span data-ttu-id="d8fba-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="d8fba-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="d8fba-142">sources</span><span class="sxs-lookup"><span data-stu-id="d8fba-142">sources</span></span>|<span data-ttu-id="d8fba-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="d8fba-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="d8fba-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="d8fba-144">Contributing policies</span></span>|
|<span data-ttu-id="d8fba-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="d8fba-145">currentValue</span></span>|<span data-ttu-id="d8fba-146">String</span><span class="sxs-lookup"><span data-stu-id="d8fba-146">String</span></span>|<span data-ttu-id="d8fba-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="d8fba-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8fba-148">Связи</span><span class="sxs-lookup"><span data-stu-id="d8fba-148">Relationships</span></span>
<span data-ttu-id="d8fba-149">Нет</span><span class="sxs-lookup"><span data-stu-id="d8fba-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8fba-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8fba-150">JSON Representation</span></span>
<span data-ttu-id="d8fba-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8fba-151">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String"
}
```




