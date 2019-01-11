---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: beed55d68c3ef7005a307d75fc1ee58ea78ed8d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845845"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="aac32-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="aac32-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="aac32-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aac32-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aac32-105">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="aac32-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="aac32-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aac32-106">Properties</span></span>
|<span data-ttu-id="aac32-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aac32-107">Property</span></span>|<span data-ttu-id="aac32-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aac32-108">Type</span></span>|<span data-ttu-id="aac32-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aac32-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac32-110">setting</span><span class="sxs-lookup"><span data-stu-id="aac32-110">setting</span></span>|<span data-ttu-id="aac32-111">String</span><span class="sxs-lookup"><span data-stu-id="aac32-111">String</span></span>|<span data-ttu-id="aac32-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="aac32-112">The setting that is being reported</span></span>|
|<span data-ttu-id="aac32-113">settingName</span><span class="sxs-lookup"><span data-stu-id="aac32-113">settingName</span></span>|<span data-ttu-id="aac32-114">String</span><span class="sxs-lookup"><span data-stu-id="aac32-114">String</span></span>|<span data-ttu-id="aac32-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="aac32-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="aac32-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="aac32-116">instanceDisplayName</span></span>|<span data-ttu-id="aac32-117">String</span><span class="sxs-lookup"><span data-stu-id="aac32-117">String</span></span>|<span data-ttu-id="aac32-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="aac32-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="aac32-119">state</span><span class="sxs-lookup"><span data-stu-id="aac32-119">state</span></span>|[<span data-ttu-id="aac32-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="aac32-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="aac32-121">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="aac32-121">The compliance state of the setting.</span></span> <span data-ttu-id="aac32-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="aac32-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="aac32-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="aac32-123">errorCode</span></span>|<span data-ttu-id="aac32-124">Int64</span><span class="sxs-lookup"><span data-stu-id="aac32-124">Int64</span></span>|<span data-ttu-id="aac32-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="aac32-125">Error code for the setting</span></span>|
|<span data-ttu-id="aac32-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="aac32-126">errorDescription</span></span>|<span data-ttu-id="aac32-127">String</span><span class="sxs-lookup"><span data-stu-id="aac32-127">String</span></span>|<span data-ttu-id="aac32-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="aac32-128">Error description</span></span>|
|<span data-ttu-id="aac32-129">userId</span><span class="sxs-lookup"><span data-stu-id="aac32-129">userId</span></span>|<span data-ttu-id="aac32-130">String</span><span class="sxs-lookup"><span data-stu-id="aac32-130">String</span></span>|<span data-ttu-id="aac32-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="aac32-131">UserId</span></span>|
|<span data-ttu-id="aac32-132">userName</span><span class="sxs-lookup"><span data-stu-id="aac32-132">userName</span></span>|<span data-ttu-id="aac32-133">String</span><span class="sxs-lookup"><span data-stu-id="aac32-133">String</span></span>|<span data-ttu-id="aac32-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="aac32-134">UserName</span></span>|
|<span data-ttu-id="aac32-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="aac32-135">userEmail</span></span>|<span data-ttu-id="aac32-136">String</span><span class="sxs-lookup"><span data-stu-id="aac32-136">String</span></span>|<span data-ttu-id="aac32-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="aac32-137">UserEmail</span></span>|
|<span data-ttu-id="aac32-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aac32-138">userPrincipalName</span></span>|<span data-ttu-id="aac32-139">String</span><span class="sxs-lookup"><span data-stu-id="aac32-139">String</span></span>|<span data-ttu-id="aac32-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="aac32-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="aac32-141">sources</span><span class="sxs-lookup"><span data-stu-id="aac32-141">sources</span></span>|<span data-ttu-id="aac32-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="aac32-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="aac32-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="aac32-143">Contributing policies</span></span>|
|<span data-ttu-id="aac32-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="aac32-144">currentValue</span></span>|<span data-ttu-id="aac32-145">String</span><span class="sxs-lookup"><span data-stu-id="aac32-145">String</span></span>|<span data-ttu-id="aac32-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="aac32-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="aac32-147">Связи</span><span class="sxs-lookup"><span data-stu-id="aac32-147">Relationships</span></span>
<span data-ttu-id="aac32-148">Нет</span><span class="sxs-lookup"><span data-stu-id="aac32-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aac32-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aac32-149">JSON Representation</span></span>
<span data-ttu-id="aac32-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aac32-150">Here is a JSON representation of the resource.</span></span>
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



