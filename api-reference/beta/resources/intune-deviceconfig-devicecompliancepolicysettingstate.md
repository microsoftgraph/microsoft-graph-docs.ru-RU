---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17930161f66ca83d59e3f2f62777a79f82b79f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425738"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="3d01e-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="3d01e-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="3d01e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d01e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d01e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d01e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d01e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d01e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d01e-107">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="3d01e-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="3d01e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d01e-108">Properties</span></span>
|<span data-ttu-id="3d01e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d01e-109">Property</span></span>|<span data-ttu-id="3d01e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3d01e-110">Type</span></span>|<span data-ttu-id="3d01e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d01e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d01e-112">setting</span><span class="sxs-lookup"><span data-stu-id="3d01e-112">setting</span></span>|<span data-ttu-id="3d01e-113">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-113">String</span></span>|<span data-ttu-id="3d01e-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="3d01e-114">The setting that is being reported</span></span>|
|<span data-ttu-id="3d01e-115">settingName</span><span class="sxs-lookup"><span data-stu-id="3d01e-115">settingName</span></span>|<span data-ttu-id="3d01e-116">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-116">String</span></span>|<span data-ttu-id="3d01e-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="3d01e-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="3d01e-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d01e-118">instanceDisplayName</span></span>|<span data-ttu-id="3d01e-119">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-119">String</span></span>|<span data-ttu-id="3d01e-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="3d01e-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="3d01e-121">state</span><span class="sxs-lookup"><span data-stu-id="3d01e-121">state</span></span>|[<span data-ttu-id="3d01e-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3d01e-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3d01e-123">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="3d01e-123">The compliance state of the setting.</span></span> <span data-ttu-id="3d01e-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3d01e-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3d01e-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="3d01e-125">errorCode</span></span>|<span data-ttu-id="3d01e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="3d01e-126">Int64</span></span>|<span data-ttu-id="3d01e-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="3d01e-127">Error code for the setting</span></span>|
|<span data-ttu-id="3d01e-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="3d01e-128">errorDescription</span></span>|<span data-ttu-id="3d01e-129">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-129">String</span></span>|<span data-ttu-id="3d01e-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="3d01e-130">Error description</span></span>|
|<span data-ttu-id="3d01e-131">userId</span><span class="sxs-lookup"><span data-stu-id="3d01e-131">userId</span></span>|<span data-ttu-id="3d01e-132">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-132">String</span></span>|<span data-ttu-id="3d01e-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="3d01e-133">UserId</span></span>|
|<span data-ttu-id="3d01e-134">userName</span><span class="sxs-lookup"><span data-stu-id="3d01e-134">userName</span></span>|<span data-ttu-id="3d01e-135">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-135">String</span></span>|<span data-ttu-id="3d01e-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="3d01e-136">UserName</span></span>|
|<span data-ttu-id="3d01e-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="3d01e-137">userEmail</span></span>|<span data-ttu-id="3d01e-138">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-138">String</span></span>|<span data-ttu-id="3d01e-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="3d01e-139">UserEmail</span></span>|
|<span data-ttu-id="3d01e-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3d01e-140">userPrincipalName</span></span>|<span data-ttu-id="3d01e-141">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-141">String</span></span>|<span data-ttu-id="3d01e-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d01e-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="3d01e-143">sources</span><span class="sxs-lookup"><span data-stu-id="3d01e-143">sources</span></span>|<span data-ttu-id="3d01e-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="3d01e-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="3d01e-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="3d01e-145">Contributing policies</span></span>|
|<span data-ttu-id="3d01e-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="3d01e-146">currentValue</span></span>|<span data-ttu-id="3d01e-147">String</span><span class="sxs-lookup"><span data-stu-id="3d01e-147">String</span></span>|<span data-ttu-id="3d01e-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="3d01e-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d01e-149">Связи</span><span class="sxs-lookup"><span data-stu-id="3d01e-149">Relationships</span></span>
<span data-ttu-id="3d01e-150">Нет</span><span class="sxs-lookup"><span data-stu-id="3d01e-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d01e-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d01e-151">JSON Representation</span></span>
<span data-ttu-id="3d01e-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d01e-152">Here is a JSON representation of the resource.</span></span>
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




