---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f24c08a2f2345f44ee4350ec5cd7d9415b2d6b5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790601"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="e9b4b-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="e9b4b-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="e9b4b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9b4b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9b4b-106">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e9b4b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9b4b-107">Properties</span></span>
|<span data-ttu-id="e9b4b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9b4b-108">Property</span></span>|<span data-ttu-id="e9b4b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e9b4b-109">Type</span></span>|<span data-ttu-id="e9b4b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9b4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9b4b-111">setting</span><span class="sxs-lookup"><span data-stu-id="e9b4b-111">setting</span></span>|<span data-ttu-id="e9b4b-112">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-112">String</span></span>|<span data-ttu-id="e9b4b-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="e9b4b-113">The setting that is being reported</span></span>|
|<span data-ttu-id="e9b4b-114">settingName</span><span class="sxs-lookup"><span data-stu-id="e9b4b-114">settingName</span></span>|<span data-ttu-id="e9b4b-115">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-115">String</span></span>|<span data-ttu-id="e9b4b-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="e9b4b-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="e9b4b-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e9b4b-117">instanceDisplayName</span></span>|<span data-ttu-id="e9b4b-118">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-118">String</span></span>|<span data-ttu-id="e9b4b-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="e9b4b-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="e9b4b-120">state</span><span class="sxs-lookup"><span data-stu-id="e9b4b-120">state</span></span>|[<span data-ttu-id="e9b4b-121">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e9b4b-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e9b4b-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-122">The compliance state of the setting.</span></span> <span data-ttu-id="e9b4b-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e9b4b-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="e9b4b-124">errorCode</span></span>|<span data-ttu-id="e9b4b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e9b4b-125">Int64</span></span>|<span data-ttu-id="e9b4b-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="e9b4b-126">Error code for the setting</span></span>|
|<span data-ttu-id="e9b4b-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e9b4b-127">errorDescription</span></span>|<span data-ttu-id="e9b4b-128">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-128">String</span></span>|<span data-ttu-id="e9b4b-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="e9b4b-129">Error description</span></span>|
|<span data-ttu-id="e9b4b-130">userId</span><span class="sxs-lookup"><span data-stu-id="e9b4b-130">userId</span></span>|<span data-ttu-id="e9b4b-131">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-131">String</span></span>|<span data-ttu-id="e9b4b-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="e9b4b-132">UserId</span></span>|
|<span data-ttu-id="e9b4b-133">userName</span><span class="sxs-lookup"><span data-stu-id="e9b4b-133">userName</span></span>|<span data-ttu-id="e9b4b-134">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-134">String</span></span>|<span data-ttu-id="e9b4b-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="e9b4b-135">UserName</span></span>|
|<span data-ttu-id="e9b4b-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="e9b4b-136">userEmail</span></span>|<span data-ttu-id="e9b4b-137">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-137">String</span></span>|<span data-ttu-id="e9b4b-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="e9b4b-138">UserEmail</span></span>|
|<span data-ttu-id="e9b4b-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9b4b-139">userPrincipalName</span></span>|<span data-ttu-id="e9b4b-140">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-140">String</span></span>|<span data-ttu-id="e9b4b-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="e9b4b-142">sources</span><span class="sxs-lookup"><span data-stu-id="e9b4b-142">sources</span></span>|<span data-ttu-id="e9b4b-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e9b4b-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e9b4b-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="e9b4b-144">Contributing policies</span></span>|
|<span data-ttu-id="e9b4b-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="e9b4b-145">currentValue</span></span>|<span data-ttu-id="e9b4b-146">String</span><span class="sxs-lookup"><span data-stu-id="e9b4b-146">String</span></span>|<span data-ttu-id="e9b4b-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="e9b4b-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9b4b-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="e9b4b-148">Relationships</span></span>
<span data-ttu-id="e9b4b-149">Нет</span><span class="sxs-lookup"><span data-stu-id="e9b4b-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9b4b-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9b4b-150">JSON Representation</span></span>
<span data-ttu-id="e9b4b-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9b4b-151">Here is a JSON representation of the resource.</span></span>
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





