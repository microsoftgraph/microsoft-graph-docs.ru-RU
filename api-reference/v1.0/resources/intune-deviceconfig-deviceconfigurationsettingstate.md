---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c50ed17421b88f2cb6137458ff853bfa92796c2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031670"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="a0b79-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="a0b79-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="a0b79-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0b79-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0b79-105">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="a0b79-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="a0b79-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0b79-106">Properties</span></span>
|<span data-ttu-id="a0b79-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0b79-107">Property</span></span>|<span data-ttu-id="a0b79-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a0b79-108">Type</span></span>|<span data-ttu-id="a0b79-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b79-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0b79-110">setting</span><span class="sxs-lookup"><span data-stu-id="a0b79-110">setting</span></span>|<span data-ttu-id="a0b79-111">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-111">String</span></span>|<span data-ttu-id="a0b79-112">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="a0b79-112">The setting that is being reported</span></span>|
|<span data-ttu-id="a0b79-113">settingName</span><span class="sxs-lookup"><span data-stu-id="a0b79-113">settingName</span></span>|<span data-ttu-id="a0b79-114">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-114">String</span></span>|<span data-ttu-id="a0b79-115">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="a0b79-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a0b79-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a0b79-116">instanceDisplayName</span></span>|<span data-ttu-id="a0b79-117">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-117">String</span></span>|<span data-ttu-id="a0b79-118">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="a0b79-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a0b79-119">state</span><span class="sxs-lookup"><span data-stu-id="a0b79-119">state</span></span>|[<span data-ttu-id="a0b79-120">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="a0b79-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a0b79-121">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="a0b79-121">The compliance state of the setting.</span></span> <span data-ttu-id="a0b79-122">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a0b79-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a0b79-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="a0b79-123">errorCode</span></span>|<span data-ttu-id="a0b79-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a0b79-124">Int64</span></span>|<span data-ttu-id="a0b79-125">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="a0b79-125">Error code for the setting</span></span>|
|<span data-ttu-id="a0b79-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a0b79-126">errorDescription</span></span>|<span data-ttu-id="a0b79-127">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-127">String</span></span>|<span data-ttu-id="a0b79-128">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="a0b79-128">Error description</span></span>|
|<span data-ttu-id="a0b79-129">userId</span><span class="sxs-lookup"><span data-stu-id="a0b79-129">userId</span></span>|<span data-ttu-id="a0b79-130">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-130">String</span></span>|<span data-ttu-id="a0b79-131">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="a0b79-131">UserId</span></span>|
|<span data-ttu-id="a0b79-132">userName</span><span class="sxs-lookup"><span data-stu-id="a0b79-132">userName</span></span>|<span data-ttu-id="a0b79-133">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-133">String</span></span>|<span data-ttu-id="a0b79-134">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a0b79-134">UserName</span></span>|
|<span data-ttu-id="a0b79-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="a0b79-135">userEmail</span></span>|<span data-ttu-id="a0b79-136">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-136">String</span></span>|<span data-ttu-id="a0b79-137">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="a0b79-137">UserEmail</span></span>|
|<span data-ttu-id="a0b79-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a0b79-138">userPrincipalName</span></span>|<span data-ttu-id="a0b79-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a0b79-139">String</span></span>|<span data-ttu-id="a0b79-140">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0b79-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="a0b79-141">sources</span><span class="sxs-lookup"><span data-stu-id="a0b79-141">sources</span></span>|<span data-ttu-id="a0b79-142">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a0b79-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a0b79-143">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="a0b79-143">Contributing policies</span></span>|
|<span data-ttu-id="a0b79-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="a0b79-144">currentValue</span></span>|<span data-ttu-id="a0b79-145">String</span><span class="sxs-lookup"><span data-stu-id="a0b79-145">String</span></span>|<span data-ttu-id="a0b79-146">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="a0b79-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0b79-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="a0b79-147">Relationships</span></span>
<span data-ttu-id="a0b79-148">Нет</span><span class="sxs-lookup"><span data-stu-id="a0b79-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0b79-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0b79-149">JSON Representation</span></span>
<span data-ttu-id="a0b79-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0b79-150">Here is a JSON representation of the resource.</span></span>
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



