---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4249866e4b6af66806d7bcc5fc6b0ab7aaa325b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793326"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="4ee08-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="4ee08-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="4ee08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ee08-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ee08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ee08-106">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="4ee08-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4ee08-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ee08-107">Properties</span></span>
|<span data-ttu-id="4ee08-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ee08-108">Property</span></span>|<span data-ttu-id="4ee08-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ee08-109">Type</span></span>|<span data-ttu-id="4ee08-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ee08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ee08-111">setting</span><span class="sxs-lookup"><span data-stu-id="4ee08-111">setting</span></span>|<span data-ttu-id="4ee08-112">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-112">String</span></span>|<span data-ttu-id="4ee08-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="4ee08-113">The setting that is being reported</span></span>|
|<span data-ttu-id="4ee08-114">settingName</span><span class="sxs-lookup"><span data-stu-id="4ee08-114">settingName</span></span>|<span data-ttu-id="4ee08-115">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-115">String</span></span>|<span data-ttu-id="4ee08-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="4ee08-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="4ee08-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4ee08-117">instanceDisplayName</span></span>|<span data-ttu-id="4ee08-118">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-118">String</span></span>|<span data-ttu-id="4ee08-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="4ee08-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="4ee08-120">state</span><span class="sxs-lookup"><span data-stu-id="4ee08-120">state</span></span>|[<span data-ttu-id="4ee08-121">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="4ee08-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4ee08-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="4ee08-122">The compliance state of the setting.</span></span> <span data-ttu-id="4ee08-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4ee08-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4ee08-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="4ee08-124">errorCode</span></span>|<span data-ttu-id="4ee08-125">Int64</span><span class="sxs-lookup"><span data-stu-id="4ee08-125">Int64</span></span>|<span data-ttu-id="4ee08-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="4ee08-126">Error code for the setting</span></span>|
|<span data-ttu-id="4ee08-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4ee08-127">errorDescription</span></span>|<span data-ttu-id="4ee08-128">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-128">String</span></span>|<span data-ttu-id="4ee08-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="4ee08-129">Error description</span></span>|
|<span data-ttu-id="4ee08-130">userId</span><span class="sxs-lookup"><span data-stu-id="4ee08-130">userId</span></span>|<span data-ttu-id="4ee08-131">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-131">String</span></span>|<span data-ttu-id="4ee08-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="4ee08-132">UserId</span></span>|
|<span data-ttu-id="4ee08-133">userName</span><span class="sxs-lookup"><span data-stu-id="4ee08-133">userName</span></span>|<span data-ttu-id="4ee08-134">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-134">String</span></span>|<span data-ttu-id="4ee08-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="4ee08-135">UserName</span></span>|
|<span data-ttu-id="4ee08-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="4ee08-136">userEmail</span></span>|<span data-ttu-id="4ee08-137">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-137">String</span></span>|<span data-ttu-id="4ee08-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="4ee08-138">UserEmail</span></span>|
|<span data-ttu-id="4ee08-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4ee08-139">userPrincipalName</span></span>|<span data-ttu-id="4ee08-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4ee08-140">String</span></span>|<span data-ttu-id="4ee08-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ee08-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="4ee08-142">sources</span><span class="sxs-lookup"><span data-stu-id="4ee08-142">sources</span></span>|<span data-ttu-id="4ee08-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="4ee08-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4ee08-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="4ee08-144">Contributing policies</span></span>|
|<span data-ttu-id="4ee08-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="4ee08-145">currentValue</span></span>|<span data-ttu-id="4ee08-146">String</span><span class="sxs-lookup"><span data-stu-id="4ee08-146">String</span></span>|<span data-ttu-id="4ee08-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="4ee08-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ee08-148">Связи</span><span class="sxs-lookup"><span data-stu-id="4ee08-148">Relationships</span></span>
<span data-ttu-id="4ee08-149">Нет</span><span class="sxs-lookup"><span data-stu-id="4ee08-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ee08-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ee08-150">JSON Representation</span></span>
<span data-ttu-id="4ee08-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee08-151">Here is a JSON representation of the resource.</span></span>
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



