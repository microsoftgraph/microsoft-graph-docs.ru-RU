---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8c508f7b936f4a04d929fe429b46ec679d7110eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822787"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="da2a2-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="da2a2-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="da2a2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da2a2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da2a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da2a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da2a2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="da2a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da2a2-107">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="da2a2-107">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="da2a2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da2a2-108">Properties</span></span>
|<span data-ttu-id="da2a2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="da2a2-109">Property</span></span>|<span data-ttu-id="da2a2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da2a2-110">Type</span></span>|<span data-ttu-id="da2a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da2a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2a2-112">setting</span><span class="sxs-lookup"><span data-stu-id="da2a2-112">setting</span></span>|<span data-ttu-id="da2a2-113">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-113">String</span></span>|<span data-ttu-id="da2a2-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="da2a2-114">The setting that is being reported</span></span>|
|<span data-ttu-id="da2a2-115">settingName</span><span class="sxs-lookup"><span data-stu-id="da2a2-115">settingName</span></span>|<span data-ttu-id="da2a2-116">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-116">String</span></span>|<span data-ttu-id="da2a2-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="da2a2-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="da2a2-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="da2a2-118">instanceDisplayName</span></span>|<span data-ttu-id="da2a2-119">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-119">String</span></span>|<span data-ttu-id="da2a2-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="da2a2-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="da2a2-121">state</span><span class="sxs-lookup"><span data-stu-id="da2a2-121">state</span></span>|[<span data-ttu-id="da2a2-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="da2a2-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="da2a2-123">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="da2a2-123">The compliance state of the setting.</span></span> <span data-ttu-id="da2a2-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="da2a2-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="da2a2-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="da2a2-125">errorCode</span></span>|<span data-ttu-id="da2a2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="da2a2-126">Int64</span></span>|<span data-ttu-id="da2a2-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="da2a2-127">Error code for the setting</span></span>|
|<span data-ttu-id="da2a2-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="da2a2-128">errorDescription</span></span>|<span data-ttu-id="da2a2-129">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-129">String</span></span>|<span data-ttu-id="da2a2-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="da2a2-130">Error description</span></span>|
|<span data-ttu-id="da2a2-131">userId</span><span class="sxs-lookup"><span data-stu-id="da2a2-131">userId</span></span>|<span data-ttu-id="da2a2-132">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-132">String</span></span>|<span data-ttu-id="da2a2-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="da2a2-133">UserId</span></span>|
|<span data-ttu-id="da2a2-134">userName</span><span class="sxs-lookup"><span data-stu-id="da2a2-134">userName</span></span>|<span data-ttu-id="da2a2-135">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-135">String</span></span>|<span data-ttu-id="da2a2-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="da2a2-136">UserName</span></span>|
|<span data-ttu-id="da2a2-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="da2a2-137">userEmail</span></span>|<span data-ttu-id="da2a2-138">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-138">String</span></span>|<span data-ttu-id="da2a2-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="da2a2-139">UserEmail</span></span>|
|<span data-ttu-id="da2a2-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="da2a2-140">userPrincipalName</span></span>|<span data-ttu-id="da2a2-141">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-141">String</span></span>|<span data-ttu-id="da2a2-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="da2a2-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="da2a2-143">sources</span><span class="sxs-lookup"><span data-stu-id="da2a2-143">sources</span></span>|<span data-ttu-id="da2a2-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="da2a2-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="da2a2-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="da2a2-145">Contributing policies</span></span>|
|<span data-ttu-id="da2a2-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="da2a2-146">currentValue</span></span>|<span data-ttu-id="da2a2-147">String</span><span class="sxs-lookup"><span data-stu-id="da2a2-147">String</span></span>|<span data-ttu-id="da2a2-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="da2a2-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="da2a2-149">Связи</span><span class="sxs-lookup"><span data-stu-id="da2a2-149">Relationships</span></span>
<span data-ttu-id="da2a2-150">Нет</span><span class="sxs-lookup"><span data-stu-id="da2a2-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da2a2-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da2a2-151">JSON Representation</span></span>
<span data-ttu-id="da2a2-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da2a2-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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





