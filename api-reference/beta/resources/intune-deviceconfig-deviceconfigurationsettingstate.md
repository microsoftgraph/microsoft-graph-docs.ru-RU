---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: tfitzmac
ms.openlocfilehash: 7ca50fe6a6186578739b166b1239a309824d1e51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316116"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="be309-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="be309-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="be309-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be309-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be309-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be309-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be309-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be309-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be309-107">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="be309-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="be309-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="be309-108">Properties</span></span>
|<span data-ttu-id="be309-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="be309-109">Property</span></span>|<span data-ttu-id="be309-110">Тип</span><span class="sxs-lookup"><span data-stu-id="be309-110">Type</span></span>|<span data-ttu-id="be309-111">Описание</span><span class="sxs-lookup"><span data-stu-id="be309-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be309-112">setting</span><span class="sxs-lookup"><span data-stu-id="be309-112">setting</span></span>|<span data-ttu-id="be309-113">String</span><span class="sxs-lookup"><span data-stu-id="be309-113">String</span></span>|<span data-ttu-id="be309-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="be309-114">The setting that is being reported</span></span>|
|<span data-ttu-id="be309-115">settingName</span><span class="sxs-lookup"><span data-stu-id="be309-115">settingName</span></span>|<span data-ttu-id="be309-116">String</span><span class="sxs-lookup"><span data-stu-id="be309-116">String</span></span>|<span data-ttu-id="be309-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="be309-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="be309-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="be309-118">instanceDisplayName</span></span>|<span data-ttu-id="be309-119">String</span><span class="sxs-lookup"><span data-stu-id="be309-119">String</span></span>|<span data-ttu-id="be309-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="be309-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="be309-121">state</span><span class="sxs-lookup"><span data-stu-id="be309-121">state</span></span>|[<span data-ttu-id="be309-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="be309-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="be309-123">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="be309-123">The compliance state of the setting.</span></span> <span data-ttu-id="be309-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="be309-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="be309-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="be309-125">errorCode</span></span>|<span data-ttu-id="be309-126">Int64</span><span class="sxs-lookup"><span data-stu-id="be309-126">Int64</span></span>|<span data-ttu-id="be309-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="be309-127">Error code for the setting</span></span>|
|<span data-ttu-id="be309-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="be309-128">errorDescription</span></span>|<span data-ttu-id="be309-129">String</span><span class="sxs-lookup"><span data-stu-id="be309-129">String</span></span>|<span data-ttu-id="be309-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="be309-130">Error description</span></span>|
|<span data-ttu-id="be309-131">userId</span><span class="sxs-lookup"><span data-stu-id="be309-131">userId</span></span>|<span data-ttu-id="be309-132">String</span><span class="sxs-lookup"><span data-stu-id="be309-132">String</span></span>|<span data-ttu-id="be309-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="be309-133">UserId</span></span>|
|<span data-ttu-id="be309-134">userName</span><span class="sxs-lookup"><span data-stu-id="be309-134">userName</span></span>|<span data-ttu-id="be309-135">String</span><span class="sxs-lookup"><span data-stu-id="be309-135">String</span></span>|<span data-ttu-id="be309-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="be309-136">UserName</span></span>|
|<span data-ttu-id="be309-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="be309-137">userEmail</span></span>|<span data-ttu-id="be309-138">String</span><span class="sxs-lookup"><span data-stu-id="be309-138">String</span></span>|<span data-ttu-id="be309-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="be309-139">UserEmail</span></span>|
|<span data-ttu-id="be309-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="be309-140">userPrincipalName</span></span>|<span data-ttu-id="be309-141">String</span><span class="sxs-lookup"><span data-stu-id="be309-141">String</span></span>|<span data-ttu-id="be309-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="be309-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="be309-143">sources</span><span class="sxs-lookup"><span data-stu-id="be309-143">sources</span></span>|<span data-ttu-id="be309-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="be309-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="be309-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="be309-145">Contributing policies</span></span>|
|<span data-ttu-id="be309-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="be309-146">currentValue</span></span>|<span data-ttu-id="be309-147">String</span><span class="sxs-lookup"><span data-stu-id="be309-147">String</span></span>|<span data-ttu-id="be309-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="be309-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="be309-149">Связи</span><span class="sxs-lookup"><span data-stu-id="be309-149">Relationships</span></span>
<span data-ttu-id="be309-150">Нет</span><span class="sxs-lookup"><span data-stu-id="be309-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be309-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be309-151">JSON Representation</span></span>
<span data-ttu-id="be309-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be309-152">Here is a JSON representation of the resource.</span></span>
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





