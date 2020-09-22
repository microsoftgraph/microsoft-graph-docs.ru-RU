---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 596fd1d59e99a2023055ec92843474a46ae20fb6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016368"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="0a518-103">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="0a518-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="0a518-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a518-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a518-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a518-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a518-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a518-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a518-107">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="0a518-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="0a518-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a518-108">Properties</span></span>
|<span data-ttu-id="0a518-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a518-109">Property</span></span>|<span data-ttu-id="0a518-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0a518-110">Type</span></span>|<span data-ttu-id="0a518-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a518-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a518-112">setting</span><span class="sxs-lookup"><span data-stu-id="0a518-112">setting</span></span>|<span data-ttu-id="0a518-113">String</span><span class="sxs-lookup"><span data-stu-id="0a518-113">String</span></span>|<span data-ttu-id="0a518-114">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="0a518-114">The setting that is being reported</span></span>|
|<span data-ttu-id="0a518-115">settingName</span><span class="sxs-lookup"><span data-stu-id="0a518-115">settingName</span></span>|<span data-ttu-id="0a518-116">String</span><span class="sxs-lookup"><span data-stu-id="0a518-116">String</span></span>|<span data-ttu-id="0a518-117">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="0a518-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="0a518-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0a518-118">instanceDisplayName</span></span>|<span data-ttu-id="0a518-119">String</span><span class="sxs-lookup"><span data-stu-id="0a518-119">String</span></span>|<span data-ttu-id="0a518-120">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="0a518-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="0a518-121">state</span><span class="sxs-lookup"><span data-stu-id="0a518-121">state</span></span>|[<span data-ttu-id="0a518-122">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="0a518-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0a518-123">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="0a518-123">The compliance state of the setting.</span></span> <span data-ttu-id="0a518-124">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0a518-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0a518-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="0a518-125">errorCode</span></span>|<span data-ttu-id="0a518-126">Int64</span><span class="sxs-lookup"><span data-stu-id="0a518-126">Int64</span></span>|<span data-ttu-id="0a518-127">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="0a518-127">Error code for the setting</span></span>|
|<span data-ttu-id="0a518-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="0a518-128">errorDescription</span></span>|<span data-ttu-id="0a518-129">String</span><span class="sxs-lookup"><span data-stu-id="0a518-129">String</span></span>|<span data-ttu-id="0a518-130">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="0a518-130">Error description</span></span>|
|<span data-ttu-id="0a518-131">userId</span><span class="sxs-lookup"><span data-stu-id="0a518-131">userId</span></span>|<span data-ttu-id="0a518-132">String</span><span class="sxs-lookup"><span data-stu-id="0a518-132">String</span></span>|<span data-ttu-id="0a518-133">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="0a518-133">UserId</span></span>|
|<span data-ttu-id="0a518-134">userName</span><span class="sxs-lookup"><span data-stu-id="0a518-134">userName</span></span>|<span data-ttu-id="0a518-135">String</span><span class="sxs-lookup"><span data-stu-id="0a518-135">String</span></span>|<span data-ttu-id="0a518-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="0a518-136">UserName</span></span>|
|<span data-ttu-id="0a518-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="0a518-137">userEmail</span></span>|<span data-ttu-id="0a518-138">String</span><span class="sxs-lookup"><span data-stu-id="0a518-138">String</span></span>|<span data-ttu-id="0a518-139">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="0a518-139">UserEmail</span></span>|
|<span data-ttu-id="0a518-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a518-140">userPrincipalName</span></span>|<span data-ttu-id="0a518-141">String</span><span class="sxs-lookup"><span data-stu-id="0a518-141">String</span></span>|<span data-ttu-id="0a518-142">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="0a518-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="0a518-143">sources</span><span class="sxs-lookup"><span data-stu-id="0a518-143">sources</span></span>|<span data-ttu-id="0a518-144">Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="0a518-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="0a518-145">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="0a518-145">Contributing policies</span></span>|
|<span data-ttu-id="0a518-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="0a518-146">currentValue</span></span>|<span data-ttu-id="0a518-147">String</span><span class="sxs-lookup"><span data-stu-id="0a518-147">String</span></span>|<span data-ttu-id="0a518-148">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="0a518-148">Current value of setting on device</span></span>|
|<span data-ttu-id="0a518-149">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="0a518-149">settingInstanceId</span></span>|<span data-ttu-id="0a518-150">String</span><span class="sxs-lookup"><span data-stu-id="0a518-150">String</span></span>|<span data-ttu-id="0a518-151">сеттингинстанцеид</span><span class="sxs-lookup"><span data-stu-id="0a518-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a518-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="0a518-152">Relationships</span></span>
<span data-ttu-id="0a518-153">Нет</span><span class="sxs-lookup"><span data-stu-id="0a518-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a518-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a518-154">JSON Representation</span></span>
<span data-ttu-id="0a518-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a518-155">Here is a JSON representation of the resource.</span></span>
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






