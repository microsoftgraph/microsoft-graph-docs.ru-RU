---
title: Тип ресурса officeClientConfiguration
description: Конфигурация клиента Office.
author: tfitzmac
ms.openlocfilehash: 67a7845a2e0327e2e5de37d424274f6e2ee35604
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303838"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="9dc8b-103">Тип ресурса officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="9dc8b-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="9dc8b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dc8b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dc8b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dc8b-107">Конфигурация клиента Office.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-107">Office Client Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="9dc8b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9dc8b-108">Methods</span></span>
|<span data-ttu-id="9dc8b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9dc8b-109">Method</span></span>|<span data-ttu-id="9dc8b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9dc8b-110">Return Type</span></span>|<span data-ttu-id="9dc8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc8b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9dc8b-112">Список officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="9dc8b-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="9dc8b-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9dc8b-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="9dc8b-114">Свойства списка и связей объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9dc8b-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9dc8b-115">Получение officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="9dc8b-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="9dc8b-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="9dc8b-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="9dc8b-117">Чтение свойства и связи объекта [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9dc8b-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9dc8b-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="9dc8b-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="9dc8b-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9dc8b-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9dc8b-120">Замените все целевые группы для политики.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="9dc8b-121">Действие updatePriorities</span><span class="sxs-lookup"><span data-stu-id="9dc8b-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="9dc8b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9dc8b-122">None</span></span>|<span data-ttu-id="9dc8b-123">Обновление политики приоритетов.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="9dc8b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dc8b-124">Properties</span></span>
|<span data-ttu-id="9dc8b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dc8b-125">Property</span></span>|<span data-ttu-id="9dc8b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc8b-126">Type</span></span>|<span data-ttu-id="9dc8b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc8b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dc8b-128">id</span><span class="sxs-lookup"><span data-stu-id="9dc8b-128">id</span></span>|<span data-ttu-id="9dc8b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="9dc8b-129">String</span></span>|<span data-ttu-id="9dc8b-130">Идентификатор политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="9dc8b-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="9dc8b-131">userPreferencePayload</span></span>|<span data-ttu-id="9dc8b-132">Stream</span><span class="sxs-lookup"><span data-stu-id="9dc8b-132">Stream</span></span>|<span data-ttu-id="9dc8b-133">Строка настройки JSON в двоичном формате, эти значения можно переопределить пользователем.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="9dc8b-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="9dc8b-134">policyPayload</span></span>|<span data-ttu-id="9dc8b-135">Stream</span><span class="sxs-lookup"><span data-stu-id="9dc8b-135">Stream</span></span>|<span data-ttu-id="9dc8b-136">Параметры политики JSON string в двоичном формате, пользователь не может изменить эти значения.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="9dc8b-137">описание</span><span class="sxs-lookup"><span data-stu-id="9dc8b-137">description</span></span>|<span data-ttu-id="9dc8b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9dc8b-138">String</span></span>|<span data-ttu-id="9dc8b-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9dc8b-139">Not yet documented</span></span>|
|<span data-ttu-id="9dc8b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9dc8b-140">displayName</span></span>|<span data-ttu-id="9dc8b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9dc8b-141">String</span></span>|<span data-ttu-id="9dc8b-142">Admin предоставляются описание клиента office конфигурации политики.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="9dc8b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc8b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9dc8b-144">DateTime.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-144">DateTime</span></span>|<span data-ttu-id="9dc8b-145">Отметка измененные даты и времени последнего политики.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="9dc8b-146">priority</span><span class="sxs-lookup"><span data-stu-id="9dc8b-146">priority</span></span>|<span data-ttu-id="9dc8b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9dc8b-147">Int32</span></span>|<span data-ttu-id="9dc8b-148">Значение приоритета должно быть уникальное значение для каждой политики в области клиента и будет использоваться для разрешения конфликтов, меньшее значение означает, что высокого приоритета.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="9dc8b-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9dc8b-149">userCheckinSummary</span></span>|[<span data-ttu-id="9dc8b-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9dc8b-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="9dc8b-151">Возврат Сводка пользователей для политики.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="9dc8b-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="9dc8b-152">checkinStatuses</span></span>|<span data-ttu-id="9dc8b-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9dc8b-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="9dc8b-154">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dc8b-155">Связи</span><span class="sxs-lookup"><span data-stu-id="9dc8b-155">Relationships</span></span>
|<span data-ttu-id="9dc8b-156">Связь</span><span class="sxs-lookup"><span data-stu-id="9dc8b-156">Relationship</span></span>|<span data-ttu-id="9dc8b-157">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc8b-157">Type</span></span>|<span data-ttu-id="9dc8b-158">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc8b-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dc8b-159">assignments</span><span class="sxs-lookup"><span data-stu-id="9dc8b-159">assignments</span></span>|<span data-ttu-id="9dc8b-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9dc8b-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9dc8b-161">Список назначений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dc8b-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dc8b-162">JSON Representation</span></span>
<span data-ttu-id="9dc8b-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dc8b-163">Here is a JSON representation of the resource.</span></span>
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



