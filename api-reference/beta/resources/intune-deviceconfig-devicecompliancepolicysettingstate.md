---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a762b9bc0e7996f1c775e372d10a60f87e649de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469517"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="8b319-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="8b319-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="8b319-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b319-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b319-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b319-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b319-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b319-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b319-107">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="8b319-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="8b319-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b319-108">Properties</span></span>
|<span data-ttu-id="8b319-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b319-109">Property</span></span>|<span data-ttu-id="8b319-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8b319-110">Type</span></span>|<span data-ttu-id="8b319-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8b319-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b319-112">setting</span><span class="sxs-lookup"><span data-stu-id="8b319-112">setting</span></span>|<span data-ttu-id="8b319-113">String</span><span class="sxs-lookup"><span data-stu-id="8b319-113">String</span></span>|<span data-ttu-id="8b319-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="8b319-114">The setting that is being reported</span></span>|
|<span data-ttu-id="8b319-115">settingName</span><span class="sxs-lookup"><span data-stu-id="8b319-115">settingName</span></span>|<span data-ttu-id="8b319-116">String</span><span class="sxs-lookup"><span data-stu-id="8b319-116">String</span></span>|<span data-ttu-id="8b319-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="8b319-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="8b319-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8b319-118">instanceDisplayName</span></span>|<span data-ttu-id="8b319-119">String</span><span class="sxs-lookup"><span data-stu-id="8b319-119">String</span></span>|<span data-ttu-id="8b319-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="8b319-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="8b319-121">state</span><span class="sxs-lookup"><span data-stu-id="8b319-121">state</span></span>|[<span data-ttu-id="8b319-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="8b319-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8b319-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="8b319-123">The compliance state of the setting.</span></span> <span data-ttu-id="8b319-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8b319-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8b319-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="8b319-125">errorCode</span></span>|<span data-ttu-id="8b319-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8b319-126">Int64</span></span>|<span data-ttu-id="8b319-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="8b319-127">Error code for the setting</span></span>|
|<span data-ttu-id="8b319-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="8b319-128">errorDescription</span></span>|<span data-ttu-id="8b319-129">String</span><span class="sxs-lookup"><span data-stu-id="8b319-129">String</span></span>|<span data-ttu-id="8b319-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="8b319-130">Error description</span></span>|
|<span data-ttu-id="8b319-131">userId</span><span class="sxs-lookup"><span data-stu-id="8b319-131">userId</span></span>|<span data-ttu-id="8b319-132">String</span><span class="sxs-lookup"><span data-stu-id="8b319-132">String</span></span>|<span data-ttu-id="8b319-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="8b319-133">UserId</span></span>|
|<span data-ttu-id="8b319-134">userName</span><span class="sxs-lookup"><span data-stu-id="8b319-134">userName</span></span>|<span data-ttu-id="8b319-135">String</span><span class="sxs-lookup"><span data-stu-id="8b319-135">String</span></span>|<span data-ttu-id="8b319-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="8b319-136">UserName</span></span>|
|<span data-ttu-id="8b319-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="8b319-137">userEmail</span></span>|<span data-ttu-id="8b319-138">String</span><span class="sxs-lookup"><span data-stu-id="8b319-138">String</span></span>|<span data-ttu-id="8b319-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="8b319-139">UserEmail</span></span>|
|<span data-ttu-id="8b319-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b319-140">userPrincipalName</span></span>|<span data-ttu-id="8b319-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8b319-141">String</span></span>|<span data-ttu-id="8b319-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b319-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="8b319-143">sources</span><span class="sxs-lookup"><span data-stu-id="8b319-143">sources</span></span>|<span data-ttu-id="8b319-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="8b319-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="8b319-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="8b319-145">Contributing policies</span></span>|
|<span data-ttu-id="8b319-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="8b319-146">currentValue</span></span>|<span data-ttu-id="8b319-147">String</span><span class="sxs-lookup"><span data-stu-id="8b319-147">String</span></span>|<span data-ttu-id="8b319-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="8b319-148">Current value of setting on device</span></span>|
|<span data-ttu-id="8b319-149">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="8b319-149">settingInstanceId</span></span>|<span data-ttu-id="8b319-150">String</span><span class="sxs-lookup"><span data-stu-id="8b319-150">String</span></span>|<span data-ttu-id="8b319-151">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="8b319-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b319-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="8b319-152">Relationships</span></span>
<span data-ttu-id="8b319-153">Нет</span><span class="sxs-lookup"><span data-stu-id="8b319-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b319-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b319-154">JSON Representation</span></span>
<span data-ttu-id="8b319-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b319-155">Here is a JSON representation of the resource.</span></span>
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
  "currentValue": "String",
  "settingInstanceId": "String"
}
```



