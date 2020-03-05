---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d5f75077fbfd29853b52adc6fc2d07b5c325905
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526631"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="e3cc3-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="e3cc3-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="e3cc3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e3cc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3cc3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3cc3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3cc3-107">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e3cc3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3cc3-108">Properties</span></span>
|<span data-ttu-id="e3cc3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3cc3-109">Property</span></span>|<span data-ttu-id="e3cc3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e3cc3-110">Type</span></span>|<span data-ttu-id="e3cc3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3cc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3cc3-112">setting</span><span class="sxs-lookup"><span data-stu-id="e3cc3-112">setting</span></span>|<span data-ttu-id="e3cc3-113">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-113">String</span></span>|<span data-ttu-id="e3cc3-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="e3cc3-114">The setting that is being reported</span></span>|
|<span data-ttu-id="e3cc3-115">settingName</span><span class="sxs-lookup"><span data-stu-id="e3cc3-115">settingName</span></span>|<span data-ttu-id="e3cc3-116">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-116">String</span></span>|<span data-ttu-id="e3cc3-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="e3cc3-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="e3cc3-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e3cc3-118">instanceDisplayName</span></span>|<span data-ttu-id="e3cc3-119">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-119">String</span></span>|<span data-ttu-id="e3cc3-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="e3cc3-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="e3cc3-121">state</span><span class="sxs-lookup"><span data-stu-id="e3cc3-121">state</span></span>|[<span data-ttu-id="e3cc3-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e3cc3-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e3cc3-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-123">The compliance state of the setting.</span></span> <span data-ttu-id="e3cc3-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e3cc3-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="e3cc3-125">errorCode</span></span>|<span data-ttu-id="e3cc3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e3cc3-126">Int64</span></span>|<span data-ttu-id="e3cc3-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="e3cc3-127">Error code for the setting</span></span>|
|<span data-ttu-id="e3cc3-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e3cc3-128">errorDescription</span></span>|<span data-ttu-id="e3cc3-129">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-129">String</span></span>|<span data-ttu-id="e3cc3-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="e3cc3-130">Error description</span></span>|
|<span data-ttu-id="e3cc3-131">userId</span><span class="sxs-lookup"><span data-stu-id="e3cc3-131">userId</span></span>|<span data-ttu-id="e3cc3-132">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-132">String</span></span>|<span data-ttu-id="e3cc3-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="e3cc3-133">UserId</span></span>|
|<span data-ttu-id="e3cc3-134">userName</span><span class="sxs-lookup"><span data-stu-id="e3cc3-134">userName</span></span>|<span data-ttu-id="e3cc3-135">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-135">String</span></span>|<span data-ttu-id="e3cc3-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="e3cc3-136">UserName</span></span>|
|<span data-ttu-id="e3cc3-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="e3cc3-137">userEmail</span></span>|<span data-ttu-id="e3cc3-138">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-138">String</span></span>|<span data-ttu-id="e3cc3-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="e3cc3-139">UserEmail</span></span>|
|<span data-ttu-id="e3cc3-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e3cc3-140">userPrincipalName</span></span>|<span data-ttu-id="e3cc3-141">Строка</span><span class="sxs-lookup"><span data-stu-id="e3cc3-141">String</span></span>|<span data-ttu-id="e3cc3-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="e3cc3-143">sources</span><span class="sxs-lookup"><span data-stu-id="e3cc3-143">sources</span></span>|<span data-ttu-id="e3cc3-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e3cc3-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e3cc3-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="e3cc3-145">Contributing policies</span></span>|
|<span data-ttu-id="e3cc3-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="e3cc3-146">currentValue</span></span>|<span data-ttu-id="e3cc3-147">String</span><span class="sxs-lookup"><span data-stu-id="e3cc3-147">String</span></span>|<span data-ttu-id="e3cc3-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="e3cc3-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3cc3-149">Связи</span><span class="sxs-lookup"><span data-stu-id="e3cc3-149">Relationships</span></span>
<span data-ttu-id="e3cc3-150">Нет</span><span class="sxs-lookup"><span data-stu-id="e3cc3-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3cc3-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3cc3-151">JSON Representation</span></span>
<span data-ttu-id="e3cc3-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3cc3-152">Here is a JSON representation of the resource.</span></span>
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



