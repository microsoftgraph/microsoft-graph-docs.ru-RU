---
title: Тип ресурса officeClientConfiguration
description: Конфигурация клиента Office.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c171f5f9f3dcedcab0d14b98a6fea0ba8fbe41eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393237"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="6a2eb-103">Тип ресурса officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a2eb-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="6a2eb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a2eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a2eb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a2eb-107">Конфигурация клиента Office.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="6a2eb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6a2eb-108">Methods</span></span>
|<span data-ttu-id="6a2eb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6a2eb-109">Method</span></span>|<span data-ttu-id="6a2eb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6a2eb-110">Return Type</span></span>|<span data-ttu-id="6a2eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a2eb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a2eb-112">Список officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="6a2eb-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="6a2eb-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6a2eb-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="6a2eb-114">Свойства списка и связей объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6a2eb-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6a2eb-115">Получение officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a2eb-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="6a2eb-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a2eb-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="6a2eb-117">Чтение свойства и связи объекта [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6a2eb-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6a2eb-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="6a2eb-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="6a2eb-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6a2eb-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6a2eb-120">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="6a2eb-121">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="6a2eb-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="6a2eb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6a2eb-122">None</span></span>|<span data-ttu-id="6a2eb-123">Обновление политики приоритетов.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a2eb-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a2eb-124">Properties</span></span>
|<span data-ttu-id="6a2eb-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a2eb-125">Property</span></span>|<span data-ttu-id="6a2eb-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6a2eb-126">Type</span></span>|<span data-ttu-id="6a2eb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6a2eb-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a2eb-128">id</span><span class="sxs-lookup"><span data-stu-id="6a2eb-128">id</span></span>|<span data-ttu-id="6a2eb-129">String</span><span class="sxs-lookup"><span data-stu-id="6a2eb-129">String</span></span>|<span data-ttu-id="6a2eb-130">Идентификатор политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="6a2eb-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="6a2eb-131">userPreferencePayload</span></span>|<span data-ttu-id="6a2eb-132">Stream</span><span class="sxs-lookup"><span data-stu-id="6a2eb-132">Stream</span></span>|<span data-ttu-id="6a2eb-133">Строка настройки JSON в двоичном формате, эти значения можно переопределить пользователем.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="6a2eb-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="6a2eb-134">policyPayload</span></span>|<span data-ttu-id="6a2eb-135">Stream</span><span class="sxs-lookup"><span data-stu-id="6a2eb-135">Stream</span></span>|<span data-ttu-id="6a2eb-136">Параметры политики JSON string в двоичном формате, пользователь не может изменить эти значения.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="6a2eb-137">description</span><span class="sxs-lookup"><span data-stu-id="6a2eb-137">description</span></span>|<span data-ttu-id="6a2eb-138">String</span><span class="sxs-lookup"><span data-stu-id="6a2eb-138">String</span></span>|<span data-ttu-id="6a2eb-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6a2eb-139">Not yet documented</span></span>|
|<span data-ttu-id="6a2eb-140">displayName</span><span class="sxs-lookup"><span data-stu-id="6a2eb-140">displayName</span></span>|<span data-ttu-id="6a2eb-141">String</span><span class="sxs-lookup"><span data-stu-id="6a2eb-141">String</span></span>|<span data-ttu-id="6a2eb-142">Admin предоставляются описание клиента office конфигурации политики.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="6a2eb-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2eb-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6a2eb-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="6a2eb-144">DateTime</span></span>|<span data-ttu-id="6a2eb-145">Отметка измененные даты и времени последнего политики.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="6a2eb-146">priority</span><span class="sxs-lookup"><span data-stu-id="6a2eb-146">priority</span></span>|<span data-ttu-id="6a2eb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6a2eb-147">Int32</span></span>|<span data-ttu-id="6a2eb-148">Значение приоритета должно быть уникальное значение для каждой политики в области клиента и будет использоваться для разрешения конфликтов, меньшее значение означает, что высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="6a2eb-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="6a2eb-149">userCheckinSummary</span></span>|[<span data-ttu-id="6a2eb-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="6a2eb-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="6a2eb-151">Возврат Сводка пользователей для политики.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="6a2eb-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="6a2eb-152">checkinStatuses</span></span>|<span data-ttu-id="6a2eb-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6a2eb-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="6a2eb-154">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a2eb-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="6a2eb-155">Relationships</span></span>
|<span data-ttu-id="6a2eb-156">Связь</span><span class="sxs-lookup"><span data-stu-id="6a2eb-156">Relationship</span></span>|<span data-ttu-id="6a2eb-157">Тип</span><span class="sxs-lookup"><span data-stu-id="6a2eb-157">Type</span></span>|<span data-ttu-id="6a2eb-158">Описание</span><span class="sxs-lookup"><span data-stu-id="6a2eb-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a2eb-159">assignments</span><span class="sxs-lookup"><span data-stu-id="6a2eb-159">assignments</span></span>|<span data-ttu-id="6a2eb-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6a2eb-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6a2eb-161">Список назначений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a2eb-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a2eb-162">JSON Representation</span></span>
<span data-ttu-id="6a2eb-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a2eb-163">Here is a JSON representation of the resource.</span></span>
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



