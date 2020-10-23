---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 555e42ca8c4a2ca419b34be32afc0f8d031d9570
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724616"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="a3ef0-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="a3ef0-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="a3ef0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3ef0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3ef0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3ef0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3ef0-107">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="a3ef0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3ef0-108">Properties</span></span>
|<span data-ttu-id="a3ef0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3ef0-109">Property</span></span>|<span data-ttu-id="a3ef0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a3ef0-110">Type</span></span>|<span data-ttu-id="a3ef0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3ef0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3ef0-112">setting</span><span class="sxs-lookup"><span data-stu-id="a3ef0-112">setting</span></span>|<span data-ttu-id="a3ef0-113">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-113">String</span></span>|<span data-ttu-id="a3ef0-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="a3ef0-114">The setting that is being reported</span></span>|
|<span data-ttu-id="a3ef0-115">settingName</span><span class="sxs-lookup"><span data-stu-id="a3ef0-115">settingName</span></span>|<span data-ttu-id="a3ef0-116">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-116">String</span></span>|<span data-ttu-id="a3ef0-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="a3ef0-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a3ef0-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3ef0-118">instanceDisplayName</span></span>|<span data-ttu-id="a3ef0-119">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-119">String</span></span>|<span data-ttu-id="a3ef0-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="a3ef0-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a3ef0-121">state</span><span class="sxs-lookup"><span data-stu-id="a3ef0-121">state</span></span>|[<span data-ttu-id="a3ef0-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="a3ef0-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a3ef0-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-123">The compliance state of the setting.</span></span> <span data-ttu-id="a3ef0-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a3ef0-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="a3ef0-125">errorCode</span></span>|<span data-ttu-id="a3ef0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a3ef0-126">Int64</span></span>|<span data-ttu-id="a3ef0-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="a3ef0-127">Error code for the setting</span></span>|
|<span data-ttu-id="a3ef0-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a3ef0-128">errorDescription</span></span>|<span data-ttu-id="a3ef0-129">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-129">String</span></span>|<span data-ttu-id="a3ef0-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="a3ef0-130">Error description</span></span>|
|<span data-ttu-id="a3ef0-131">userId</span><span class="sxs-lookup"><span data-stu-id="a3ef0-131">userId</span></span>|<span data-ttu-id="a3ef0-132">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-132">String</span></span>|<span data-ttu-id="a3ef0-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="a3ef0-133">UserId</span></span>|
|<span data-ttu-id="a3ef0-134">userName</span><span class="sxs-lookup"><span data-stu-id="a3ef0-134">userName</span></span>|<span data-ttu-id="a3ef0-135">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-135">String</span></span>|<span data-ttu-id="a3ef0-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a3ef0-136">UserName</span></span>|
|<span data-ttu-id="a3ef0-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="a3ef0-137">userEmail</span></span>|<span data-ttu-id="a3ef0-138">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-138">String</span></span>|<span data-ttu-id="a3ef0-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="a3ef0-139">UserEmail</span></span>|
|<span data-ttu-id="a3ef0-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3ef0-140">userPrincipalName</span></span>|<span data-ttu-id="a3ef0-141">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-141">String</span></span>|<span data-ttu-id="a3ef0-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="a3ef0-143">sources</span><span class="sxs-lookup"><span data-stu-id="a3ef0-143">sources</span></span>|<span data-ttu-id="a3ef0-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a3ef0-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a3ef0-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="a3ef0-145">Contributing policies</span></span>|
|<span data-ttu-id="a3ef0-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="a3ef0-146">currentValue</span></span>|<span data-ttu-id="a3ef0-147">String</span><span class="sxs-lookup"><span data-stu-id="a3ef0-147">String</span></span>|<span data-ttu-id="a3ef0-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="a3ef0-148">Current value of setting on device</span></span>|
|<span data-ttu-id="a3ef0-149">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="a3ef0-149">settingInstanceId</span></span>|<span data-ttu-id="a3ef0-150">Строка</span><span class="sxs-lookup"><span data-stu-id="a3ef0-150">String</span></span>|<span data-ttu-id="a3ef0-151">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="a3ef0-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3ef0-152">Связи</span><span class="sxs-lookup"><span data-stu-id="a3ef0-152">Relationships</span></span>
<span data-ttu-id="a3ef0-153">Нет</span><span class="sxs-lookup"><span data-stu-id="a3ef0-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3ef0-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3ef0-154">JSON Representation</span></span>
<span data-ttu-id="a3ef0-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3ef0-155">Here is a JSON representation of the resource.</span></span>
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
  "currentValue": "String",
  "settingInstanceId": "String"
}
```





