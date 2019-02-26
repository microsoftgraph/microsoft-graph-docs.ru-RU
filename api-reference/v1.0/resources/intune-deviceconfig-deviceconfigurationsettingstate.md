---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d79d4c35572c98c82f80f8903d42cfa3b983c2e9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252905"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="3a2d8-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="3a2d8-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="3a2d8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a2d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a2d8-105">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="3a2d8-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="3a2d8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a2d8-106">Properties</span></span>
|<span data-ttu-id="3a2d8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a2d8-107">Property</span></span>|<span data-ttu-id="3a2d8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3a2d8-108">Type</span></span>|<span data-ttu-id="3a2d8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2d8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a2d8-110">setting</span><span class="sxs-lookup"><span data-stu-id="3a2d8-110">setting</span></span>|<span data-ttu-id="3a2d8-111">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-111">String</span></span>|<span data-ttu-id="3a2d8-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="3a2d8-112">The setting that is being reported</span></span>|
|<span data-ttu-id="3a2d8-113">settingName</span><span class="sxs-lookup"><span data-stu-id="3a2d8-113">settingName</span></span>|<span data-ttu-id="3a2d8-114">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-114">String</span></span>|<span data-ttu-id="3a2d8-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="3a2d8-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="3a2d8-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a2d8-116">instanceDisplayName</span></span>|<span data-ttu-id="3a2d8-117">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-117">String</span></span>|<span data-ttu-id="3a2d8-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="3a2d8-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="3a2d8-119">state</span><span class="sxs-lookup"><span data-stu-id="3a2d8-119">state</span></span>|[<span data-ttu-id="3a2d8-120">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="3a2d8-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3a2d8-121">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="3a2d8-121">The compliance state of the setting.</span></span> <span data-ttu-id="3a2d8-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3a2d8-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3a2d8-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="3a2d8-123">errorCode</span></span>|<span data-ttu-id="3a2d8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3a2d8-124">Int64</span></span>|<span data-ttu-id="3a2d8-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="3a2d8-125">Error code for the setting</span></span>|
|<span data-ttu-id="3a2d8-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="3a2d8-126">errorDescription</span></span>|<span data-ttu-id="3a2d8-127">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-127">String</span></span>|<span data-ttu-id="3a2d8-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="3a2d8-128">Error description</span></span>|
|<span data-ttu-id="3a2d8-129">userId</span><span class="sxs-lookup"><span data-stu-id="3a2d8-129">userId</span></span>|<span data-ttu-id="3a2d8-130">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-130">String</span></span>|<span data-ttu-id="3a2d8-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="3a2d8-131">UserId</span></span>|
|<span data-ttu-id="3a2d8-132">userName</span><span class="sxs-lookup"><span data-stu-id="3a2d8-132">userName</span></span>|<span data-ttu-id="3a2d8-133">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-133">String</span></span>|<span data-ttu-id="3a2d8-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="3a2d8-134">UserName</span></span>|
|<span data-ttu-id="3a2d8-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="3a2d8-135">userEmail</span></span>|<span data-ttu-id="3a2d8-136">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-136">String</span></span>|<span data-ttu-id="3a2d8-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="3a2d8-137">UserEmail</span></span>|
|<span data-ttu-id="3a2d8-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a2d8-138">userPrincipalName</span></span>|<span data-ttu-id="3a2d8-139">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-139">String</span></span>|<span data-ttu-id="3a2d8-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="3a2d8-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="3a2d8-141">sources</span><span class="sxs-lookup"><span data-stu-id="3a2d8-141">sources</span></span>|<span data-ttu-id="3a2d8-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="3a2d8-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="3a2d8-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="3a2d8-143">Contributing policies</span></span>|
|<span data-ttu-id="3a2d8-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="3a2d8-144">currentValue</span></span>|<span data-ttu-id="3a2d8-145">String</span><span class="sxs-lookup"><span data-stu-id="3a2d8-145">String</span></span>|<span data-ttu-id="3a2d8-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="3a2d8-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a2d8-147">Связи</span><span class="sxs-lookup"><span data-stu-id="3a2d8-147">Relationships</span></span>
<span data-ttu-id="3a2d8-148">Нет</span><span class="sxs-lookup"><span data-stu-id="3a2d8-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a2d8-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a2d8-149">JSON Representation</span></span>
<span data-ttu-id="3a2d8-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a2d8-150">Here is a JSON representation of the resource.</span></span>
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



