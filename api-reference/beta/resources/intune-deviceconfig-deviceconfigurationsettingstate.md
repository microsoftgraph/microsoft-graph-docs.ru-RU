---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e5c62cbd5ef1daa3adf0ba03931bc65b2b6d9b2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995954"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="193f9-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="193f9-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="193f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="193f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="193f9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="193f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="193f9-106">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="193f9-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="193f9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="193f9-107">Properties</span></span>
|<span data-ttu-id="193f9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="193f9-108">Property</span></span>|<span data-ttu-id="193f9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="193f9-109">Type</span></span>|<span data-ttu-id="193f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="193f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="193f9-111">setting</span><span class="sxs-lookup"><span data-stu-id="193f9-111">setting</span></span>|<span data-ttu-id="193f9-112">String</span><span class="sxs-lookup"><span data-stu-id="193f9-112">String</span></span>|<span data-ttu-id="193f9-113">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="193f9-113">The setting that is being reported</span></span>|
|<span data-ttu-id="193f9-114">settingName</span><span class="sxs-lookup"><span data-stu-id="193f9-114">settingName</span></span>|<span data-ttu-id="193f9-115">String</span><span class="sxs-lookup"><span data-stu-id="193f9-115">String</span></span>|<span data-ttu-id="193f9-116">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="193f9-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="193f9-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="193f9-117">instanceDisplayName</span></span>|<span data-ttu-id="193f9-118">String</span><span class="sxs-lookup"><span data-stu-id="193f9-118">String</span></span>|<span data-ttu-id="193f9-119">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="193f9-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="193f9-120">state</span><span class="sxs-lookup"><span data-stu-id="193f9-120">state</span></span>|[<span data-ttu-id="193f9-121">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="193f9-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="193f9-122">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="193f9-122">The compliance state of the setting.</span></span> <span data-ttu-id="193f9-123">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="193f9-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="193f9-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="193f9-124">errorCode</span></span>|<span data-ttu-id="193f9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="193f9-125">Int64</span></span>|<span data-ttu-id="193f9-126">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="193f9-126">Error code for the setting</span></span>|
|<span data-ttu-id="193f9-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="193f9-127">errorDescription</span></span>|<span data-ttu-id="193f9-128">String</span><span class="sxs-lookup"><span data-stu-id="193f9-128">String</span></span>|<span data-ttu-id="193f9-129">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="193f9-129">Error description</span></span>|
|<span data-ttu-id="193f9-130">userId</span><span class="sxs-lookup"><span data-stu-id="193f9-130">userId</span></span>|<span data-ttu-id="193f9-131">String</span><span class="sxs-lookup"><span data-stu-id="193f9-131">String</span></span>|<span data-ttu-id="193f9-132">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="193f9-132">UserId</span></span>|
|<span data-ttu-id="193f9-133">userName</span><span class="sxs-lookup"><span data-stu-id="193f9-133">userName</span></span>|<span data-ttu-id="193f9-134">String</span><span class="sxs-lookup"><span data-stu-id="193f9-134">String</span></span>|<span data-ttu-id="193f9-135">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="193f9-135">UserName</span></span>|
|<span data-ttu-id="193f9-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="193f9-136">userEmail</span></span>|<span data-ttu-id="193f9-137">String</span><span class="sxs-lookup"><span data-stu-id="193f9-137">String</span></span>|<span data-ttu-id="193f9-138">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="193f9-138">UserEmail</span></span>|
|<span data-ttu-id="193f9-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="193f9-139">userPrincipalName</span></span>|<span data-ttu-id="193f9-140">Строка</span><span class="sxs-lookup"><span data-stu-id="193f9-140">String</span></span>|<span data-ttu-id="193f9-141">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="193f9-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="193f9-142">sources</span><span class="sxs-lookup"><span data-stu-id="193f9-142">sources</span></span>|<span data-ttu-id="193f9-143">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="193f9-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="193f9-144">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="193f9-144">Contributing policies</span></span>|
|<span data-ttu-id="193f9-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="193f9-145">currentValue</span></span>|<span data-ttu-id="193f9-146">String</span><span class="sxs-lookup"><span data-stu-id="193f9-146">String</span></span>|<span data-ttu-id="193f9-147">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="193f9-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="193f9-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="193f9-148">Relationships</span></span>
<span data-ttu-id="193f9-149">Нет</span><span class="sxs-lookup"><span data-stu-id="193f9-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="193f9-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="193f9-150">JSON Representation</span></span>
<span data-ttu-id="193f9-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="193f9-151">Here is a JSON representation of the resource.</span></span>
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





