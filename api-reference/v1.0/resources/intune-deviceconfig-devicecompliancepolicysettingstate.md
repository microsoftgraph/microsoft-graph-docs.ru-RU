---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: tfitzmac
ms.openlocfilehash: 3dcd63327a3518314619cd7add6ac6f23e69396b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320372"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="0ce60-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="0ce60-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="0ce60-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ce60-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ce60-105">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="0ce60-105">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="0ce60-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ce60-106">Properties</span></span>
|<span data-ttu-id="0ce60-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ce60-107">Property</span></span>|<span data-ttu-id="0ce60-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0ce60-108">Type</span></span>|<span data-ttu-id="0ce60-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce60-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ce60-110">setting</span><span class="sxs-lookup"><span data-stu-id="0ce60-110">setting</span></span>|<span data-ttu-id="0ce60-111">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-111">String</span></span>|<span data-ttu-id="0ce60-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="0ce60-112">The setting that is being reported</span></span>|
|<span data-ttu-id="0ce60-113">settingName</span><span class="sxs-lookup"><span data-stu-id="0ce60-113">settingName</span></span>|<span data-ttu-id="0ce60-114">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-114">String</span></span>|<span data-ttu-id="0ce60-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="0ce60-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="0ce60-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ce60-116">instanceDisplayName</span></span>|<span data-ttu-id="0ce60-117">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-117">String</span></span>|<span data-ttu-id="0ce60-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="0ce60-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="0ce60-119">state</span><span class="sxs-lookup"><span data-stu-id="0ce60-119">state</span></span>|[<span data-ttu-id="0ce60-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0ce60-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0ce60-121">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="0ce60-121">The compliance state of the setting.</span></span> <span data-ttu-id="0ce60-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0ce60-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0ce60-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="0ce60-123">errorCode</span></span>|<span data-ttu-id="0ce60-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0ce60-124">Int64</span></span>|<span data-ttu-id="0ce60-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="0ce60-125">Error code for the setting</span></span>|
|<span data-ttu-id="0ce60-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="0ce60-126">errorDescription</span></span>|<span data-ttu-id="0ce60-127">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-127">String</span></span>|<span data-ttu-id="0ce60-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="0ce60-128">Error description</span></span>|
|<span data-ttu-id="0ce60-129">userId</span><span class="sxs-lookup"><span data-stu-id="0ce60-129">userId</span></span>|<span data-ttu-id="0ce60-130">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-130">String</span></span>|<span data-ttu-id="0ce60-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="0ce60-131">UserId</span></span>|
|<span data-ttu-id="0ce60-132">userName</span><span class="sxs-lookup"><span data-stu-id="0ce60-132">userName</span></span>|<span data-ttu-id="0ce60-133">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-133">String</span></span>|<span data-ttu-id="0ce60-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="0ce60-134">UserName</span></span>|
|<span data-ttu-id="0ce60-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="0ce60-135">userEmail</span></span>|<span data-ttu-id="0ce60-136">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-136">String</span></span>|<span data-ttu-id="0ce60-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="0ce60-137">UserEmail</span></span>|
|<span data-ttu-id="0ce60-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ce60-138">userPrincipalName</span></span>|<span data-ttu-id="0ce60-139">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-139">String</span></span>|<span data-ttu-id="0ce60-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="0ce60-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="0ce60-141">sources</span><span class="sxs-lookup"><span data-stu-id="0ce60-141">sources</span></span>|<span data-ttu-id="0ce60-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="0ce60-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="0ce60-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="0ce60-143">Contributing policies</span></span>|
|<span data-ttu-id="0ce60-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="0ce60-144">currentValue</span></span>|<span data-ttu-id="0ce60-145">String</span><span class="sxs-lookup"><span data-stu-id="0ce60-145">String</span></span>|<span data-ttu-id="0ce60-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="0ce60-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ce60-147">Связи</span><span class="sxs-lookup"><span data-stu-id="0ce60-147">Relationships</span></span>
<span data-ttu-id="0ce60-148">Нет</span><span class="sxs-lookup"><span data-stu-id="0ce60-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ce60-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ce60-149">JSON Representation</span></span>
<span data-ttu-id="0ce60-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ce60-150">Here is a JSON representation of the resource.</span></span>
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



