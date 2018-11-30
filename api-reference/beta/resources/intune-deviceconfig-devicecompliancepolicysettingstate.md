---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
ms.openlocfilehash: d73cbe591e30e465065e0c446c6d98d7232a049c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080118"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="5535f-103">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="5535f-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="5535f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5535f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5535f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5535f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5535f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5535f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5535f-107">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="5535f-107">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="5535f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5535f-108">Properties</span></span>
|<span data-ttu-id="5535f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5535f-109">Property</span></span>|<span data-ttu-id="5535f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5535f-110">Type</span></span>|<span data-ttu-id="5535f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5535f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5535f-112">setting</span><span class="sxs-lookup"><span data-stu-id="5535f-112">setting</span></span>|<span data-ttu-id="5535f-113">String</span><span class="sxs-lookup"><span data-stu-id="5535f-113">String</span></span>|<span data-ttu-id="5535f-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="5535f-114">The setting that is being reported</span></span>|
|<span data-ttu-id="5535f-115">settingName</span><span class="sxs-lookup"><span data-stu-id="5535f-115">settingName</span></span>|<span data-ttu-id="5535f-116">String</span><span class="sxs-lookup"><span data-stu-id="5535f-116">String</span></span>|<span data-ttu-id="5535f-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="5535f-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="5535f-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5535f-118">instanceDisplayName</span></span>|<span data-ttu-id="5535f-119">String</span><span class="sxs-lookup"><span data-stu-id="5535f-119">String</span></span>|<span data-ttu-id="5535f-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="5535f-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="5535f-121">state</span><span class="sxs-lookup"><span data-stu-id="5535f-121">state</span></span>|[<span data-ttu-id="5535f-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5535f-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5535f-123">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="5535f-123">The compliance state of the setting.</span></span> <span data-ttu-id="5535f-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5535f-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5535f-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="5535f-125">errorCode</span></span>|<span data-ttu-id="5535f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5535f-126">Int64</span></span>|<span data-ttu-id="5535f-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="5535f-127">Error code for the setting</span></span>|
|<span data-ttu-id="5535f-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="5535f-128">errorDescription</span></span>|<span data-ttu-id="5535f-129">String</span><span class="sxs-lookup"><span data-stu-id="5535f-129">String</span></span>|<span data-ttu-id="5535f-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="5535f-130">Error description</span></span>|
|<span data-ttu-id="5535f-131">userId</span><span class="sxs-lookup"><span data-stu-id="5535f-131">userId</span></span>|<span data-ttu-id="5535f-132">String</span><span class="sxs-lookup"><span data-stu-id="5535f-132">String</span></span>|<span data-ttu-id="5535f-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="5535f-133">UserId</span></span>|
|<span data-ttu-id="5535f-134">userName</span><span class="sxs-lookup"><span data-stu-id="5535f-134">userName</span></span>|<span data-ttu-id="5535f-135">String</span><span class="sxs-lookup"><span data-stu-id="5535f-135">String</span></span>|<span data-ttu-id="5535f-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="5535f-136">UserName</span></span>|
|<span data-ttu-id="5535f-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="5535f-137">userEmail</span></span>|<span data-ttu-id="5535f-138">String</span><span class="sxs-lookup"><span data-stu-id="5535f-138">String</span></span>|<span data-ttu-id="5535f-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="5535f-139">UserEmail</span></span>|
|<span data-ttu-id="5535f-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5535f-140">userPrincipalName</span></span>|<span data-ttu-id="5535f-141">String</span><span class="sxs-lookup"><span data-stu-id="5535f-141">String</span></span>|<span data-ttu-id="5535f-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="5535f-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="5535f-143">sources</span><span class="sxs-lookup"><span data-stu-id="5535f-143">sources</span></span>|<span data-ttu-id="5535f-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="5535f-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="5535f-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="5535f-145">Contributing policies</span></span>|
|<span data-ttu-id="5535f-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="5535f-146">currentValue</span></span>|<span data-ttu-id="5535f-147">String</span><span class="sxs-lookup"><span data-stu-id="5535f-147">String</span></span>|<span data-ttu-id="5535f-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="5535f-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="5535f-149">Связи</span><span class="sxs-lookup"><span data-stu-id="5535f-149">Relationships</span></span>
<span data-ttu-id="5535f-150">Нет</span><span class="sxs-lookup"><span data-stu-id="5535f-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5535f-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5535f-151">JSON Representation</span></span>
<span data-ttu-id="5535f-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5535f-152">Here is a JSON representation of the resource.</span></span>
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





