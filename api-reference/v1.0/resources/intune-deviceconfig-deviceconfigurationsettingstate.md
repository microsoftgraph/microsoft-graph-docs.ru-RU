---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
ms.openlocfilehash: 056d4e1b501d438feb5bbda6b7910c9998c73cdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026205"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="51443-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="51443-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="51443-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51443-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51443-105">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="51443-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="51443-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51443-106">Properties</span></span>
|<span data-ttu-id="51443-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51443-107">Property</span></span>|<span data-ttu-id="51443-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51443-108">Type</span></span>|<span data-ttu-id="51443-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51443-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51443-110">setting</span><span class="sxs-lookup"><span data-stu-id="51443-110">setting</span></span>|<span data-ttu-id="51443-111">String</span><span class="sxs-lookup"><span data-stu-id="51443-111">String</span></span>|<span data-ttu-id="51443-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="51443-112">The setting that is being reported</span></span>|
|<span data-ttu-id="51443-113">settingName</span><span class="sxs-lookup"><span data-stu-id="51443-113">settingName</span></span>|<span data-ttu-id="51443-114">String</span><span class="sxs-lookup"><span data-stu-id="51443-114">String</span></span>|<span data-ttu-id="51443-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="51443-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="51443-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="51443-116">instanceDisplayName</span></span>|<span data-ttu-id="51443-117">String</span><span class="sxs-lookup"><span data-stu-id="51443-117">String</span></span>|<span data-ttu-id="51443-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="51443-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="51443-119">state</span><span class="sxs-lookup"><span data-stu-id="51443-119">state</span></span>|[<span data-ttu-id="51443-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="51443-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="51443-121">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="51443-121">The compliance state of the setting.</span></span> <span data-ttu-id="51443-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="51443-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="51443-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="51443-123">errorCode</span></span>|<span data-ttu-id="51443-124">Int64</span><span class="sxs-lookup"><span data-stu-id="51443-124">Int64</span></span>|<span data-ttu-id="51443-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="51443-125">Error code for the setting</span></span>|
|<span data-ttu-id="51443-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="51443-126">errorDescription</span></span>|<span data-ttu-id="51443-127">String</span><span class="sxs-lookup"><span data-stu-id="51443-127">String</span></span>|<span data-ttu-id="51443-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="51443-128">Error description</span></span>|
|<span data-ttu-id="51443-129">userId</span><span class="sxs-lookup"><span data-stu-id="51443-129">userId</span></span>|<span data-ttu-id="51443-130">String</span><span class="sxs-lookup"><span data-stu-id="51443-130">String</span></span>|<span data-ttu-id="51443-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="51443-131">UserId</span></span>|
|<span data-ttu-id="51443-132">userName</span><span class="sxs-lookup"><span data-stu-id="51443-132">userName</span></span>|<span data-ttu-id="51443-133">String</span><span class="sxs-lookup"><span data-stu-id="51443-133">String</span></span>|<span data-ttu-id="51443-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="51443-134">UserName</span></span>|
|<span data-ttu-id="51443-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="51443-135">userEmail</span></span>|<span data-ttu-id="51443-136">String</span><span class="sxs-lookup"><span data-stu-id="51443-136">String</span></span>|<span data-ttu-id="51443-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="51443-137">UserEmail</span></span>|
|<span data-ttu-id="51443-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51443-138">userPrincipalName</span></span>|<span data-ttu-id="51443-139">String</span><span class="sxs-lookup"><span data-stu-id="51443-139">String</span></span>|<span data-ttu-id="51443-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="51443-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="51443-141">sources</span><span class="sxs-lookup"><span data-stu-id="51443-141">sources</span></span>|<span data-ttu-id="51443-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="51443-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="51443-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="51443-143">Contributing policies</span></span>|
|<span data-ttu-id="51443-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="51443-144">currentValue</span></span>|<span data-ttu-id="51443-145">String</span><span class="sxs-lookup"><span data-stu-id="51443-145">String</span></span>|<span data-ttu-id="51443-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="51443-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="51443-147">Связи</span><span class="sxs-lookup"><span data-stu-id="51443-147">Relationships</span></span>
<span data-ttu-id="51443-148">Нет</span><span class="sxs-lookup"><span data-stu-id="51443-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51443-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51443-149">JSON Representation</span></span>
<span data-ttu-id="51443-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51443-150">Here is a JSON representation of the resource.</span></span>
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



