---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bf91b3acef707bafc33d1498486ed45c9fc4793
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199401"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="a2783-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="a2783-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="a2783-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2783-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2783-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2783-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2783-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2783-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2783-107">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="a2783-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="a2783-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2783-108">Properties</span></span>
|<span data-ttu-id="a2783-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2783-109">Property</span></span>|<span data-ttu-id="a2783-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a2783-110">Type</span></span>|<span data-ttu-id="a2783-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a2783-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2783-112">setting</span><span class="sxs-lookup"><span data-stu-id="a2783-112">setting</span></span>|<span data-ttu-id="a2783-113">String</span><span class="sxs-lookup"><span data-stu-id="a2783-113">String</span></span>|<span data-ttu-id="a2783-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="a2783-114">The setting that is being reported</span></span>|
|<span data-ttu-id="a2783-115">settingName</span><span class="sxs-lookup"><span data-stu-id="a2783-115">settingName</span></span>|<span data-ttu-id="a2783-116">String</span><span class="sxs-lookup"><span data-stu-id="a2783-116">String</span></span>|<span data-ttu-id="a2783-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="a2783-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a2783-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a2783-118">instanceDisplayName</span></span>|<span data-ttu-id="a2783-119">String</span><span class="sxs-lookup"><span data-stu-id="a2783-119">String</span></span>|<span data-ttu-id="a2783-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="a2783-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a2783-121">state</span><span class="sxs-lookup"><span data-stu-id="a2783-121">state</span></span>|[<span data-ttu-id="a2783-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="a2783-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a2783-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="a2783-123">The compliance state of the setting.</span></span> <span data-ttu-id="a2783-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a2783-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a2783-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="a2783-125">errorCode</span></span>|<span data-ttu-id="a2783-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a2783-126">Int64</span></span>|<span data-ttu-id="a2783-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="a2783-127">Error code for the setting</span></span>|
|<span data-ttu-id="a2783-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a2783-128">errorDescription</span></span>|<span data-ttu-id="a2783-129">String</span><span class="sxs-lookup"><span data-stu-id="a2783-129">String</span></span>|<span data-ttu-id="a2783-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="a2783-130">Error description</span></span>|
|<span data-ttu-id="a2783-131">userId</span><span class="sxs-lookup"><span data-stu-id="a2783-131">userId</span></span>|<span data-ttu-id="a2783-132">String</span><span class="sxs-lookup"><span data-stu-id="a2783-132">String</span></span>|<span data-ttu-id="a2783-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="a2783-133">UserId</span></span>|
|<span data-ttu-id="a2783-134">userName</span><span class="sxs-lookup"><span data-stu-id="a2783-134">userName</span></span>|<span data-ttu-id="a2783-135">String</span><span class="sxs-lookup"><span data-stu-id="a2783-135">String</span></span>|<span data-ttu-id="a2783-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a2783-136">UserName</span></span>|
|<span data-ttu-id="a2783-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="a2783-137">userEmail</span></span>|<span data-ttu-id="a2783-138">String</span><span class="sxs-lookup"><span data-stu-id="a2783-138">String</span></span>|<span data-ttu-id="a2783-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="a2783-139">UserEmail</span></span>|
|<span data-ttu-id="a2783-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2783-140">userPrincipalName</span></span>|<span data-ttu-id="a2783-141">String</span><span class="sxs-lookup"><span data-stu-id="a2783-141">String</span></span>|<span data-ttu-id="a2783-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2783-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="a2783-143">sources</span><span class="sxs-lookup"><span data-stu-id="a2783-143">sources</span></span>|<span data-ttu-id="a2783-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a2783-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a2783-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="a2783-145">Contributing policies</span></span>|
|<span data-ttu-id="a2783-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="a2783-146">currentValue</span></span>|<span data-ttu-id="a2783-147">String</span><span class="sxs-lookup"><span data-stu-id="a2783-147">String</span></span>|<span data-ttu-id="a2783-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="a2783-148">Current value of setting on device</span></span>|
|<span data-ttu-id="a2783-149">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="a2783-149">settingInstanceId</span></span>|<span data-ttu-id="a2783-150">String</span><span class="sxs-lookup"><span data-stu-id="a2783-150">String</span></span>|<span data-ttu-id="a2783-151">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="a2783-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2783-152">Связи</span><span class="sxs-lookup"><span data-stu-id="a2783-152">Relationships</span></span>
<span data-ttu-id="a2783-153">Нет</span><span class="sxs-lookup"><span data-stu-id="a2783-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2783-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2783-154">JSON Representation</span></span>
<span data-ttu-id="a2783-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2783-155">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```




