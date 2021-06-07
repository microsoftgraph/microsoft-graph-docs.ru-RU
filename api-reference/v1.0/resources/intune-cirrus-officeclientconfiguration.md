---
title: тип ресурса officeClientConfiguration
description: Office Конфигурация клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 181e06de36176c5d2dbbdb8d1794ae64390ee71b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753127"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="aae13-103">тип ресурса officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="aae13-103">officeClientConfiguration resource type</span></span>

<span data-ttu-id="aae13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aae13-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aae13-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aae13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aae13-107">Office Конфигурация клиента.</span><span class="sxs-lookup"><span data-stu-id="aae13-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="aae13-108">Методы</span><span class="sxs-lookup"><span data-stu-id="aae13-108">Methods</span></span>
|<span data-ttu-id="aae13-109">Метод</span><span class="sxs-lookup"><span data-stu-id="aae13-109">Method</span></span>|<span data-ttu-id="aae13-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aae13-110">Return Type</span></span>|<span data-ttu-id="aae13-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aae13-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aae13-112">Список officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="aae13-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="aae13-113">[коллекция officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aae13-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="aae13-114">Список свойств и связей объектов [officeClientConfiguration.](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aae13-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="aae13-115">Получить officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="aae13-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="aae13-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="aae13-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="aae13-117">Чтение свойств и связей объекта [officeClientConfiguration.](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aae13-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="aae13-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="aae13-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="aae13-119">[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aae13-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aae13-120">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="aae13-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="aae13-121">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="aae13-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="aae13-122">Нет</span><span class="sxs-lookup"><span data-stu-id="aae13-122">None</span></span>|<span data-ttu-id="aae13-123">Обновление приоритетов политики.</span><span class="sxs-lookup"><span data-stu-id="aae13-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="aae13-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="aae13-124">Properties</span></span>
|<span data-ttu-id="aae13-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="aae13-125">Property</span></span>|<span data-ttu-id="aae13-126">Тип</span><span class="sxs-lookup"><span data-stu-id="aae13-126">Type</span></span>|<span data-ttu-id="aae13-127">Описание</span><span class="sxs-lookup"><span data-stu-id="aae13-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae13-128">id</span><span class="sxs-lookup"><span data-stu-id="aae13-128">id</span></span>|<span data-ttu-id="aae13-129">String</span><span class="sxs-lookup"><span data-stu-id="aae13-129">String</span></span>|<span data-ttu-id="aae13-130">Id политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="aae13-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="aae13-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="aae13-131">userPreferencePayload</span></span>|<span data-ttu-id="aae13-132">Stream</span><span class="sxs-lookup"><span data-stu-id="aae13-132">Stream</span></span>|<span data-ttu-id="aae13-133">Параметры параметров JSON строки в двоичном формате, эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="aae13-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="aae13-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="aae13-134">policyPayload</span></span>|<span data-ttu-id="aae13-135">Stream</span><span class="sxs-lookup"><span data-stu-id="aae13-135">Stream</span></span>|<span data-ttu-id="aae13-136">Параметры JSON строки JSON в двоичном формате, эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="aae13-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="aae13-137">description</span><span class="sxs-lookup"><span data-stu-id="aae13-137">description</span></span>|<span data-ttu-id="aae13-138">String</span><span class="sxs-lookup"><span data-stu-id="aae13-138">String</span></span>|<span data-ttu-id="aae13-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="aae13-139">Not yet documented</span></span>|
|<span data-ttu-id="aae13-140">displayName</span><span class="sxs-lookup"><span data-stu-id="aae13-140">displayName</span></span>|<span data-ttu-id="aae13-141">String</span><span class="sxs-lookup"><span data-stu-id="aae13-141">String</span></span>|<span data-ttu-id="aae13-142">Администратор предоставил описание политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="aae13-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="aae13-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aae13-143">lastModifiedDateTime</span></span>|<span data-ttu-id="aae13-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="aae13-144">DateTime</span></span>|<span data-ttu-id="aae13-145">Последний измененный штамп даты политики.</span><span class="sxs-lookup"><span data-stu-id="aae13-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="aae13-146">priority</span><span class="sxs-lookup"><span data-stu-id="aae13-146">priority</span></span>|<span data-ttu-id="aae13-147">Int32</span><span class="sxs-lookup"><span data-stu-id="aae13-147">Int32</span></span>|<span data-ttu-id="aae13-148">Значение приоритета должно быть уникальным значением для каждой политики клиента и использоваться для разрешения конфликтов, более низкие значения означают высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="aae13-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="aae13-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="aae13-149">userCheckinSummary</span></span>|[<span data-ttu-id="aae13-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="aae13-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="aae13-151">Сводка регистрации пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="aae13-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="aae13-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="aae13-152">checkinStatuses</span></span>|<span data-ttu-id="aae13-153">[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="aae13-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="aae13-154">Список состояния регистрации клиента office.</span><span class="sxs-lookup"><span data-stu-id="aae13-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aae13-155">Связи</span><span class="sxs-lookup"><span data-stu-id="aae13-155">Relationships</span></span>
|<span data-ttu-id="aae13-156">Связь</span><span class="sxs-lookup"><span data-stu-id="aae13-156">Relationship</span></span>|<span data-ttu-id="aae13-157">Тип</span><span class="sxs-lookup"><span data-stu-id="aae13-157">Type</span></span>|<span data-ttu-id="aae13-158">Описание</span><span class="sxs-lookup"><span data-stu-id="aae13-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae13-159">assignments</span><span class="sxs-lookup"><span data-stu-id="aae13-159">assignments</span></span>|<span data-ttu-id="aae13-160">[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aae13-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aae13-161">Список групповых назначений для политики.</span><span class="sxs-lookup"><span data-stu-id="aae13-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aae13-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aae13-162">JSON Representation</span></span>
<span data-ttu-id="aae13-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aae13-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```




