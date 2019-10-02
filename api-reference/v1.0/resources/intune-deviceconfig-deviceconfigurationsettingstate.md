---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47bbca9073765b5f7a09827b5b1eecb44ba81b6e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359490"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="b9a25-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="b9a25-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="b9a25-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9a25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a25-105">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="b9a25-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b9a25-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9a25-106">Properties</span></span>
|<span data-ttu-id="b9a25-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9a25-107">Property</span></span>|<span data-ttu-id="b9a25-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b9a25-108">Type</span></span>|<span data-ttu-id="b9a25-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a25-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a25-110">setting</span><span class="sxs-lookup"><span data-stu-id="b9a25-110">setting</span></span>|<span data-ttu-id="b9a25-111">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-111">String</span></span>|<span data-ttu-id="b9a25-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="b9a25-112">The setting that is being reported</span></span>|
|<span data-ttu-id="b9a25-113">settingName</span><span class="sxs-lookup"><span data-stu-id="b9a25-113">settingName</span></span>|<span data-ttu-id="b9a25-114">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-114">String</span></span>|<span data-ttu-id="b9a25-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="b9a25-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b9a25-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b9a25-116">instanceDisplayName</span></span>|<span data-ttu-id="b9a25-117">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-117">String</span></span>|<span data-ttu-id="b9a25-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="b9a25-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b9a25-119">state</span><span class="sxs-lookup"><span data-stu-id="b9a25-119">state</span></span>|[<span data-ttu-id="b9a25-120">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="b9a25-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b9a25-121">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="b9a25-121">The compliance state of the setting.</span></span> <span data-ttu-id="b9a25-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b9a25-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b9a25-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="b9a25-123">errorCode</span></span>|<span data-ttu-id="b9a25-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b9a25-124">Int64</span></span>|<span data-ttu-id="b9a25-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="b9a25-125">Error code for the setting</span></span>|
|<span data-ttu-id="b9a25-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b9a25-126">errorDescription</span></span>|<span data-ttu-id="b9a25-127">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-127">String</span></span>|<span data-ttu-id="b9a25-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="b9a25-128">Error description</span></span>|
|<span data-ttu-id="b9a25-129">userId</span><span class="sxs-lookup"><span data-stu-id="b9a25-129">userId</span></span>|<span data-ttu-id="b9a25-130">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-130">String</span></span>|<span data-ttu-id="b9a25-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="b9a25-131">UserId</span></span>|
|<span data-ttu-id="b9a25-132">userName</span><span class="sxs-lookup"><span data-stu-id="b9a25-132">userName</span></span>|<span data-ttu-id="b9a25-133">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-133">String</span></span>|<span data-ttu-id="b9a25-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b9a25-134">UserName</span></span>|
|<span data-ttu-id="b9a25-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="b9a25-135">userEmail</span></span>|<span data-ttu-id="b9a25-136">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-136">String</span></span>|<span data-ttu-id="b9a25-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="b9a25-137">UserEmail</span></span>|
|<span data-ttu-id="b9a25-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9a25-138">userPrincipalName</span></span>|<span data-ttu-id="b9a25-139">Строка</span><span class="sxs-lookup"><span data-stu-id="b9a25-139">String</span></span>|<span data-ttu-id="b9a25-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9a25-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="b9a25-141">sources</span><span class="sxs-lookup"><span data-stu-id="b9a25-141">sources</span></span>|<span data-ttu-id="b9a25-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="b9a25-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b9a25-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="b9a25-143">Contributing policies</span></span>|
|<span data-ttu-id="b9a25-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="b9a25-144">currentValue</span></span>|<span data-ttu-id="b9a25-145">String</span><span class="sxs-lookup"><span data-stu-id="b9a25-145">String</span></span>|<span data-ttu-id="b9a25-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="b9a25-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9a25-147">Связи</span><span class="sxs-lookup"><span data-stu-id="b9a25-147">Relationships</span></span>
<span data-ttu-id="b9a25-148">Нет</span><span class="sxs-lookup"><span data-stu-id="b9a25-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9a25-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9a25-149">JSON Representation</span></span>
<span data-ttu-id="b9a25-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9a25-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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




