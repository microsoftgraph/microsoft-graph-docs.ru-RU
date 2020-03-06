---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aafa0147bac2acfcaa1f77291be1451c907b2f72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530770"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="18d8e-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="18d8e-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="18d8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d8e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18d8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d8e-106">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="18d8e-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="18d8e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="18d8e-107">Properties</span></span>
|<span data-ttu-id="18d8e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="18d8e-108">Property</span></span>|<span data-ttu-id="18d8e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="18d8e-109">Type</span></span>|<span data-ttu-id="18d8e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18d8e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d8e-111">setting</span><span class="sxs-lookup"><span data-stu-id="18d8e-111">setting</span></span>|<span data-ttu-id="18d8e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-112">String</span></span>|<span data-ttu-id="18d8e-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="18d8e-113">The setting that is being reported</span></span>|
|<span data-ttu-id="18d8e-114">settingName</span><span class="sxs-lookup"><span data-stu-id="18d8e-114">settingName</span></span>|<span data-ttu-id="18d8e-115">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-115">String</span></span>|<span data-ttu-id="18d8e-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="18d8e-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="18d8e-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="18d8e-117">instanceDisplayName</span></span>|<span data-ttu-id="18d8e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-118">String</span></span>|<span data-ttu-id="18d8e-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="18d8e-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="18d8e-120">state</span><span class="sxs-lookup"><span data-stu-id="18d8e-120">state</span></span>|[<span data-ttu-id="18d8e-121">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="18d8e-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="18d8e-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="18d8e-122">The compliance state of the setting.</span></span> <span data-ttu-id="18d8e-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="18d8e-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="18d8e-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="18d8e-124">errorCode</span></span>|<span data-ttu-id="18d8e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="18d8e-125">Int64</span></span>|<span data-ttu-id="18d8e-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="18d8e-126">Error code for the setting</span></span>|
|<span data-ttu-id="18d8e-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="18d8e-127">errorDescription</span></span>|<span data-ttu-id="18d8e-128">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-128">String</span></span>|<span data-ttu-id="18d8e-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="18d8e-129">Error description</span></span>|
|<span data-ttu-id="18d8e-130">userId</span><span class="sxs-lookup"><span data-stu-id="18d8e-130">userId</span></span>|<span data-ttu-id="18d8e-131">String</span><span class="sxs-lookup"><span data-stu-id="18d8e-131">String</span></span>|<span data-ttu-id="18d8e-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="18d8e-132">UserId</span></span>|
|<span data-ttu-id="18d8e-133">userName</span><span class="sxs-lookup"><span data-stu-id="18d8e-133">userName</span></span>|<span data-ttu-id="18d8e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-134">String</span></span>|<span data-ttu-id="18d8e-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="18d8e-135">UserName</span></span>|
|<span data-ttu-id="18d8e-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="18d8e-136">userEmail</span></span>|<span data-ttu-id="18d8e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-137">String</span></span>|<span data-ttu-id="18d8e-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="18d8e-138">UserEmail</span></span>|
|<span data-ttu-id="18d8e-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="18d8e-139">userPrincipalName</span></span>|<span data-ttu-id="18d8e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="18d8e-140">String</span></span>|<span data-ttu-id="18d8e-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="18d8e-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="18d8e-142">sources</span><span class="sxs-lookup"><span data-stu-id="18d8e-142">sources</span></span>|<span data-ttu-id="18d8e-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="18d8e-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="18d8e-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="18d8e-144">Contributing policies</span></span>|
|<span data-ttu-id="18d8e-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="18d8e-145">currentValue</span></span>|<span data-ttu-id="18d8e-146">String</span><span class="sxs-lookup"><span data-stu-id="18d8e-146">String</span></span>|<span data-ttu-id="18d8e-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="18d8e-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="18d8e-148">Связи</span><span class="sxs-lookup"><span data-stu-id="18d8e-148">Relationships</span></span>
<span data-ttu-id="18d8e-149">Нет</span><span class="sxs-lookup"><span data-stu-id="18d8e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18d8e-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18d8e-150">JSON Representation</span></span>
<span data-ttu-id="18d8e-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18d8e-151">Here is a JSON representation of the resource.</span></span>
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




