---
title: Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате
description: Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9f5fbdae9a59b19216db0db0f460402ce3ba374a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437294"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="be788-103">Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате</span><span class="sxs-lookup"><span data-stu-id="be788-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="be788-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be788-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be788-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be788-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be788-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be788-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be788-107">Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="be788-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="be788-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="be788-108">Properties</span></span>
|<span data-ttu-id="be788-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="be788-109">Property</span></span>|<span data-ttu-id="be788-110">Тип</span><span class="sxs-lookup"><span data-stu-id="be788-110">Type</span></span>|<span data-ttu-id="be788-111">Описание</span><span class="sxs-lookup"><span data-stu-id="be788-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be788-112">setting</span><span class="sxs-lookup"><span data-stu-id="be788-112">setting</span></span>|<span data-ttu-id="be788-113">String</span><span class="sxs-lookup"><span data-stu-id="be788-113">String</span></span>|<span data-ttu-id="be788-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="be788-114">The setting that is being reported</span></span>|
|<span data-ttu-id="be788-115">settingName</span><span class="sxs-lookup"><span data-stu-id="be788-115">settingName</span></span>|<span data-ttu-id="be788-116">String</span><span class="sxs-lookup"><span data-stu-id="be788-116">String</span></span>|<span data-ttu-id="be788-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="be788-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="be788-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="be788-118">instanceDisplayName</span></span>|<span data-ttu-id="be788-119">String</span><span class="sxs-lookup"><span data-stu-id="be788-119">String</span></span>|<span data-ttu-id="be788-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="be788-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="be788-121">state</span><span class="sxs-lookup"><span data-stu-id="be788-121">state</span></span>|[<span data-ttu-id="be788-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="be788-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="be788-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="be788-123">The compliance state of the setting.</span></span> <span data-ttu-id="be788-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="be788-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="be788-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="be788-125">errorCode</span></span>|<span data-ttu-id="be788-126">Int64</span><span class="sxs-lookup"><span data-stu-id="be788-126">Int64</span></span>|<span data-ttu-id="be788-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="be788-127">Error code for the setting</span></span>|
|<span data-ttu-id="be788-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="be788-128">errorDescription</span></span>|<span data-ttu-id="be788-129">String</span><span class="sxs-lookup"><span data-stu-id="be788-129">String</span></span>|<span data-ttu-id="be788-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="be788-130">Error description</span></span>|
|<span data-ttu-id="be788-131">userId</span><span class="sxs-lookup"><span data-stu-id="be788-131">userId</span></span>|<span data-ttu-id="be788-132">String</span><span class="sxs-lookup"><span data-stu-id="be788-132">String</span></span>|<span data-ttu-id="be788-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="be788-133">UserId</span></span>|
|<span data-ttu-id="be788-134">userName</span><span class="sxs-lookup"><span data-stu-id="be788-134">userName</span></span>|<span data-ttu-id="be788-135">String</span><span class="sxs-lookup"><span data-stu-id="be788-135">String</span></span>|<span data-ttu-id="be788-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="be788-136">UserName</span></span>|
|<span data-ttu-id="be788-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="be788-137">userEmail</span></span>|<span data-ttu-id="be788-138">String</span><span class="sxs-lookup"><span data-stu-id="be788-138">String</span></span>|<span data-ttu-id="be788-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="be788-139">UserEmail</span></span>|
|<span data-ttu-id="be788-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="be788-140">userPrincipalName</span></span>|<span data-ttu-id="be788-141">Строка</span><span class="sxs-lookup"><span data-stu-id="be788-141">String</span></span>|<span data-ttu-id="be788-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="be788-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="be788-143">sources</span><span class="sxs-lookup"><span data-stu-id="be788-143">sources</span></span>|<span data-ttu-id="be788-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="be788-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="be788-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="be788-145">Contributing policies</span></span>|
|<span data-ttu-id="be788-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="be788-146">currentValue</span></span>|<span data-ttu-id="be788-147">String</span><span class="sxs-lookup"><span data-stu-id="be788-147">String</span></span>|<span data-ttu-id="be788-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="be788-148">Current value of setting on device</span></span>|
|<span data-ttu-id="be788-149">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="be788-149">settingInstanceId</span></span>|<span data-ttu-id="be788-150">String</span><span class="sxs-lookup"><span data-stu-id="be788-150">String</span></span>|<span data-ttu-id="be788-151">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="be788-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="be788-152">Связи</span><span class="sxs-lookup"><span data-stu-id="be788-152">Relationships</span></span>
<span data-ttu-id="be788-153">Нет</span><span class="sxs-lookup"><span data-stu-id="be788-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be788-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be788-154">JSON Representation</span></span>
<span data-ttu-id="be788-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be788-155">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```



