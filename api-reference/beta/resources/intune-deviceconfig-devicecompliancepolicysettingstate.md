---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27288df13fecbe7cc85b455d1df30b4885b17eec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333102"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="697f1-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="697f1-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="697f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="697f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="697f1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="697f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="697f1-106">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="697f1-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="697f1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="697f1-107">Properties</span></span>
|<span data-ttu-id="697f1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="697f1-108">Property</span></span>|<span data-ttu-id="697f1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="697f1-109">Type</span></span>|<span data-ttu-id="697f1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="697f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="697f1-111">setting</span><span class="sxs-lookup"><span data-stu-id="697f1-111">setting</span></span>|<span data-ttu-id="697f1-112">String</span><span class="sxs-lookup"><span data-stu-id="697f1-112">String</span></span>|<span data-ttu-id="697f1-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="697f1-113">The setting that is being reported</span></span>|
|<span data-ttu-id="697f1-114">settingName</span><span class="sxs-lookup"><span data-stu-id="697f1-114">settingName</span></span>|<span data-ttu-id="697f1-115">String</span><span class="sxs-lookup"><span data-stu-id="697f1-115">String</span></span>|<span data-ttu-id="697f1-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="697f1-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="697f1-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="697f1-117">instanceDisplayName</span></span>|<span data-ttu-id="697f1-118">String</span><span class="sxs-lookup"><span data-stu-id="697f1-118">String</span></span>|<span data-ttu-id="697f1-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="697f1-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="697f1-120">state</span><span class="sxs-lookup"><span data-stu-id="697f1-120">state</span></span>|[<span data-ttu-id="697f1-121">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="697f1-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="697f1-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="697f1-122">The compliance state of the setting.</span></span> <span data-ttu-id="697f1-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="697f1-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="697f1-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="697f1-124">errorCode</span></span>|<span data-ttu-id="697f1-125">Int64</span><span class="sxs-lookup"><span data-stu-id="697f1-125">Int64</span></span>|<span data-ttu-id="697f1-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="697f1-126">Error code for the setting</span></span>|
|<span data-ttu-id="697f1-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="697f1-127">errorDescription</span></span>|<span data-ttu-id="697f1-128">String</span><span class="sxs-lookup"><span data-stu-id="697f1-128">String</span></span>|<span data-ttu-id="697f1-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="697f1-129">Error description</span></span>|
|<span data-ttu-id="697f1-130">userId</span><span class="sxs-lookup"><span data-stu-id="697f1-130">userId</span></span>|<span data-ttu-id="697f1-131">String</span><span class="sxs-lookup"><span data-stu-id="697f1-131">String</span></span>|<span data-ttu-id="697f1-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="697f1-132">UserId</span></span>|
|<span data-ttu-id="697f1-133">userName</span><span class="sxs-lookup"><span data-stu-id="697f1-133">userName</span></span>|<span data-ttu-id="697f1-134">String</span><span class="sxs-lookup"><span data-stu-id="697f1-134">String</span></span>|<span data-ttu-id="697f1-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="697f1-135">UserName</span></span>|
|<span data-ttu-id="697f1-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="697f1-136">userEmail</span></span>|<span data-ttu-id="697f1-137">String</span><span class="sxs-lookup"><span data-stu-id="697f1-137">String</span></span>|<span data-ttu-id="697f1-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="697f1-138">UserEmail</span></span>|
|<span data-ttu-id="697f1-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="697f1-139">userPrincipalName</span></span>|<span data-ttu-id="697f1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="697f1-140">String</span></span>|<span data-ttu-id="697f1-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="697f1-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="697f1-142">sources</span><span class="sxs-lookup"><span data-stu-id="697f1-142">sources</span></span>|<span data-ttu-id="697f1-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="697f1-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="697f1-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="697f1-144">Contributing policies</span></span>|
|<span data-ttu-id="697f1-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="697f1-145">currentValue</span></span>|<span data-ttu-id="697f1-146">String</span><span class="sxs-lookup"><span data-stu-id="697f1-146">String</span></span>|<span data-ttu-id="697f1-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="697f1-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="697f1-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="697f1-148">Relationships</span></span>
<span data-ttu-id="697f1-149">Нет</span><span class="sxs-lookup"><span data-stu-id="697f1-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="697f1-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="697f1-150">JSON Representation</span></span>
<span data-ttu-id="697f1-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="697f1-151">Here is a JSON representation of the resource.</span></span>
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



