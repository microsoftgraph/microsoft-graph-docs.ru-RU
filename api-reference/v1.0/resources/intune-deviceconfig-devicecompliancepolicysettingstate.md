---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f4eb50b7cbae1eccb2f5797de2186c5d51f48ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448864"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="4b8b0-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="4b8b0-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="4b8b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b8b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b8b0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b8b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b8b0-106">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="4b8b0-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4b8b0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b8b0-107">Properties</span></span>
|<span data-ttu-id="4b8b0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b8b0-108">Property</span></span>|<span data-ttu-id="4b8b0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b8b0-109">Type</span></span>|<span data-ttu-id="4b8b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b8b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b8b0-111">setting</span><span class="sxs-lookup"><span data-stu-id="4b8b0-111">setting</span></span>|<span data-ttu-id="4b8b0-112">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-112">String</span></span>|<span data-ttu-id="4b8b0-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="4b8b0-113">The setting that is being reported</span></span>|
|<span data-ttu-id="4b8b0-114">settingName</span><span class="sxs-lookup"><span data-stu-id="4b8b0-114">settingName</span></span>|<span data-ttu-id="4b8b0-115">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-115">String</span></span>|<span data-ttu-id="4b8b0-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="4b8b0-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="4b8b0-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4b8b0-117">instanceDisplayName</span></span>|<span data-ttu-id="4b8b0-118">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-118">String</span></span>|<span data-ttu-id="4b8b0-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="4b8b0-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="4b8b0-120">state</span><span class="sxs-lookup"><span data-stu-id="4b8b0-120">state</span></span>|[<span data-ttu-id="4b8b0-121">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="4b8b0-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4b8b0-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="4b8b0-122">The compliance state of the setting.</span></span> <span data-ttu-id="4b8b0-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4b8b0-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4b8b0-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="4b8b0-124">errorCode</span></span>|<span data-ttu-id="4b8b0-125">Int64</span><span class="sxs-lookup"><span data-stu-id="4b8b0-125">Int64</span></span>|<span data-ttu-id="4b8b0-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="4b8b0-126">Error code for the setting</span></span>|
|<span data-ttu-id="4b8b0-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4b8b0-127">errorDescription</span></span>|<span data-ttu-id="4b8b0-128">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-128">String</span></span>|<span data-ttu-id="4b8b0-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="4b8b0-129">Error description</span></span>|
|<span data-ttu-id="4b8b0-130">userId</span><span class="sxs-lookup"><span data-stu-id="4b8b0-130">userId</span></span>|<span data-ttu-id="4b8b0-131">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-131">String</span></span>|<span data-ttu-id="4b8b0-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="4b8b0-132">UserId</span></span>|
|<span data-ttu-id="4b8b0-133">userName</span><span class="sxs-lookup"><span data-stu-id="4b8b0-133">userName</span></span>|<span data-ttu-id="4b8b0-134">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-134">String</span></span>|<span data-ttu-id="4b8b0-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="4b8b0-135">UserName</span></span>|
|<span data-ttu-id="4b8b0-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="4b8b0-136">userEmail</span></span>|<span data-ttu-id="4b8b0-137">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-137">String</span></span>|<span data-ttu-id="4b8b0-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="4b8b0-138">UserEmail</span></span>|
|<span data-ttu-id="4b8b0-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b8b0-139">userPrincipalName</span></span>|<span data-ttu-id="4b8b0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4b8b0-140">String</span></span>|<span data-ttu-id="4b8b0-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b8b0-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="4b8b0-142">sources</span><span class="sxs-lookup"><span data-stu-id="4b8b0-142">sources</span></span>|<span data-ttu-id="4b8b0-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="4b8b0-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4b8b0-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="4b8b0-144">Contributing policies</span></span>|
|<span data-ttu-id="4b8b0-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="4b8b0-145">currentValue</span></span>|<span data-ttu-id="4b8b0-146">String</span><span class="sxs-lookup"><span data-stu-id="4b8b0-146">String</span></span>|<span data-ttu-id="4b8b0-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="4b8b0-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b8b0-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="4b8b0-148">Relationships</span></span>
<span data-ttu-id="4b8b0-149">Нет</span><span class="sxs-lookup"><span data-stu-id="4b8b0-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b8b0-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b8b0-150">JSON Representation</span></span>
<span data-ttu-id="4b8b0-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b8b0-151">Here is a JSON representation of the resource.</span></span>
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







