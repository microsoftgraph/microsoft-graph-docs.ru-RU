---
title: Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате
description: Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 23b1b82efef9ecead0a129c5906acbf129790d08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010208"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="fe3c4-103">Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате</span><span class="sxs-lookup"><span data-stu-id="fe3c4-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="fe3c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe3c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe3c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe3c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe3c4-107">Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="fe3c4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe3c4-108">Properties</span></span>
|<span data-ttu-id="fe3c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe3c4-109">Property</span></span>|<span data-ttu-id="fe3c4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fe3c4-110">Type</span></span>|<span data-ttu-id="fe3c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe3c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3c4-112">setting</span><span class="sxs-lookup"><span data-stu-id="fe3c4-112">setting</span></span>|<span data-ttu-id="fe3c4-113">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-113">String</span></span>|<span data-ttu-id="fe3c4-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="fe3c4-114">The setting that is being reported</span></span>|
|<span data-ttu-id="fe3c4-115">settingName</span><span class="sxs-lookup"><span data-stu-id="fe3c4-115">settingName</span></span>|<span data-ttu-id="fe3c4-116">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-116">String</span></span>|<span data-ttu-id="fe3c4-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="fe3c4-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="fe3c4-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe3c4-118">instanceDisplayName</span></span>|<span data-ttu-id="fe3c4-119">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-119">String</span></span>|<span data-ttu-id="fe3c4-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="fe3c4-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="fe3c4-121">state</span><span class="sxs-lookup"><span data-stu-id="fe3c4-121">state</span></span>|[<span data-ttu-id="fe3c4-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="fe3c4-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fe3c4-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-123">The compliance state of the setting.</span></span> <span data-ttu-id="fe3c4-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fe3c4-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="fe3c4-125">errorCode</span></span>|<span data-ttu-id="fe3c4-126">Int64</span><span class="sxs-lookup"><span data-stu-id="fe3c4-126">Int64</span></span>|<span data-ttu-id="fe3c4-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="fe3c4-127">Error code for the setting</span></span>|
|<span data-ttu-id="fe3c4-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="fe3c4-128">errorDescription</span></span>|<span data-ttu-id="fe3c4-129">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-129">String</span></span>|<span data-ttu-id="fe3c4-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="fe3c4-130">Error description</span></span>|
|<span data-ttu-id="fe3c4-131">userId</span><span class="sxs-lookup"><span data-stu-id="fe3c4-131">userId</span></span>|<span data-ttu-id="fe3c4-132">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-132">String</span></span>|<span data-ttu-id="fe3c4-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="fe3c4-133">UserId</span></span>|
|<span data-ttu-id="fe3c4-134">userName</span><span class="sxs-lookup"><span data-stu-id="fe3c4-134">userName</span></span>|<span data-ttu-id="fe3c4-135">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-135">String</span></span>|<span data-ttu-id="fe3c4-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="fe3c4-136">UserName</span></span>|
|<span data-ttu-id="fe3c4-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="fe3c4-137">userEmail</span></span>|<span data-ttu-id="fe3c4-138">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-138">String</span></span>|<span data-ttu-id="fe3c4-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="fe3c4-139">UserEmail</span></span>|
|<span data-ttu-id="fe3c4-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe3c4-140">userPrincipalName</span></span>|<span data-ttu-id="fe3c4-141">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-141">String</span></span>|<span data-ttu-id="fe3c4-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="fe3c4-143">sources</span><span class="sxs-lookup"><span data-stu-id="fe3c4-143">sources</span></span>|<span data-ttu-id="fe3c4-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="fe3c4-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="fe3c4-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="fe3c4-145">Contributing policies</span></span>|
|<span data-ttu-id="fe3c4-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="fe3c4-146">currentValue</span></span>|<span data-ttu-id="fe3c4-147">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-147">String</span></span>|<span data-ttu-id="fe3c4-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="fe3c4-148">Current value of setting on device</span></span>|
|<span data-ttu-id="fe3c4-149">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="fe3c4-149">settingInstanceId</span></span>|<span data-ttu-id="fe3c4-150">String</span><span class="sxs-lookup"><span data-stu-id="fe3c4-150">String</span></span>|<span data-ttu-id="fe3c4-151">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="fe3c4-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe3c4-152">Связи</span><span class="sxs-lookup"><span data-stu-id="fe3c4-152">Relationships</span></span>
<span data-ttu-id="fe3c4-153">Нет</span><span class="sxs-lookup"><span data-stu-id="fe3c4-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe3c4-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe3c4-154">JSON Representation</span></span>
<span data-ttu-id="fe3c4-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe3c4-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
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






